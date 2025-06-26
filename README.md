# Simple CRUD example written in Go

The application was testend and build on go version go1.24.2 linux/amd64

## Build the app
Building before running
```
    go build
```
## Run the server
Run the app with the following command
```
    go run .
```
## Test the endpoints
You've got some operations that you can test

GET
```
    curl -X GET http://localhost:8080/movies
```

POST
```
    curl -X POST http://localhost:8080/movies \
    -H "Content-Type: application/json"
    -d '{ISBN:"Some-isbn", Title: "Some-title", Director: {Firstname: "Some",Lastname: "Director"}}'
```

DELETE
```
    curl -X DELETE http://localhost:8080/movies/{id}
```

PUT
```
    curl -X PUT http://localhost:8080/movies/{id} \
    -H "Content-Type: application/json"
    -d '{ISBN:"Some-isbn", Title: "Some-title", Director: {Firstname: "Some",Lastname: "Director"}}'
```
