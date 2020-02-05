# graphql-demo
A demo app showing how to provide GraphQL functionality with graphql-java and Spring Boot

# Build and run
`
$ gradlew clean build
$ gradlew bootRun
`

# Example
```
POST /graphql
Host: localhost:8080

{"query":"query {bookById(id: \"book-1\") {
    name,
    pageCount,
    author {
      firstName,
      lastName
    }
   }
 }"
}
```
