# graphql-demo
A demo app showing how to provide GraphQL functionality with graphql-java and Spring Boot

# Build and run
`
$ gradlew clean build
$ gradlew bootRun
`

# Example
```
POST /graphql HTTP/1.1
Host: localhost:8080
Content-Type: application/json

{"query":"query {\n    bookById(id: \"book-1\") {\n        name,\n        pageCount,\n        author {\n            firstName,\n            lastName\n        }\n    }\n}","variables":{}}

```
