# Curl-Cheat-Sheet
Curl command references

## GET request: 
- `curl -o response.json -v http://app-url:port/getEmployee?employee_id=1`

### GET request with headers and query parameters:
- `curl --header "Content-Type:application/json" --header "employee_id:51" http://app-url:port/getEmployee?employee_id`

## POST request with form parameters:
- `curl curl -d 'employee_id=abc123&employee_name=trump' http://app-url:port/createEmployee`

### POST request with response body from file:
- `curl -d @request.json -H "Content-Type: application/json" http://app-url:port/createEmployee`

### POST request with JSON body:
- `curl --data "{\"employee_id\":\"test1\",\"employee_name\":\"newone\"}" --header "Content-Type:application/json" http://app-url:port/createEmployee`
