# Employee
The code provides a REST API for an employee entity using Spring Boot, JPA and Hibernate.

Following endpoints have been provided:

Retrieve all Employees - @GetMapping(“/employees”)  

Get details of specific employee - @GetMapping(“/employees/{id}”)

Delete a employee - @DeleteMapping(“/employees/{id}”)

Create a new employee - @PostMapping(“/employees”)

Update employee details - @PutMapping(“/employees/{id}”)


<b> POST Request: </b>

curl --location --request POST 'http://localhost:8080/employees' \
--header 'Content-Type: application/json' \
--data-raw '    {
        "name": "saba"
    }'
    
    
<b> GET Request: </b>

curl --location --request GET 'http://localhost:8080/employees'


curl --location --request GET 'http://localhost:8080/employees/1'

<b> PUT Request: </b>

curl --location --request PUT 'http://localhost:8080/employees/1' \
--header 'Content-Type: application/json' \
--data-raw '{
    "name": "naila"
}'

<b> DELETE Request: </b>

curl --location --request DELETE 'http://localhost:8080/employees/1'

    
