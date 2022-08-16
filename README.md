Golang HRMS APIs with MongoDB. Create, read, update and delete HR employee with Postman. 

## Technologies Used
* Golang
* MongoDB
* Postman


## Dependencies
* Install Go - https://go.dev/doc/install
* Install MongoDB - https://www.mongodb.com/try/download/community
* Install Postman - https://www.postman.com/downloads/


## Executing program
* Download the repository to your computer, go to project file, and run the code
```
git clone https://github.com/sayedh/go-mongoDB-HRMS
cd go-mongoDB-HRMS
go mod tidy
go run main.go
```

* Test APIs with Postman
  * Create a POST request to add data with http://localhost:3000/employee
  ```
  {
    "name":"Sayed Haque",
    "salary":1234567,
    "city":"Los Angeles"
  }
  ```
  * Create a GET request to get all data with http://localhost:3000/employee
  * Create a PUT request to update employee data with http://localhost:3000/employee/627af1fa0903ad2cbc8f6c21 (<-- the 627xxxxxxx is the ID of the data, can be changed to desired data that needs to be updated)
  ```
  {
    "name":"Sayed Haque",
    "salary":87654321,
    "city":"Los Angeles"
  }
  ```
  * Create a DELETE request with http://localhost:3000/employee/627af1fa0903ad2cbc8f6c21 (<-- the 627xxxxxxx is the ID of the data, can be changed to desired data that needs to be deleted)
