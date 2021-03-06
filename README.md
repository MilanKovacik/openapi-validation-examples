# openapi-validation-examples
Examples of JSR303 validation with OpenAPI

[OpenAPI Specification](https://swagger.io/docs/specification/about/)

## How to build:
### Build the Spring REST-API Backend app
`./gradlew clean build`

### Start docker compose (Edge router + Swagger UI + Spring REST-API Backend app)
`docker-compose up --build`

### Access Swagger UI
[localhost:3000/swagger-ui](localhost:3000/swagger-ui)

How to try locally POST endpoint:
Servlet API:
`curl -X POST -H "content-type: application/json" -d "@payload/employeeVacation.json" localhost:8090/api/employees/1/vacations -v`

WebFlux API:
`curl -X POST -H "content-type: application/json" -d "@payload/employeeVacation.json" localhost:8093/api/employees/1/vacations -v`

Coroutines API:
`curl -X POST -H "content-type: application/json" -d "@payload/employeeVacation.json" localhost:8095/api/employees/1/vacations -v`


# Links
- [https://openapi.tools]()
- [springdoc library](https://github.com/springdoc/springdoc-openapi)
- [reDoc](https://github.com/Redocly/redoc)
- ReDoc aggregation of more specs ([reDocMoreSpecs](https://github.com/volbrene/redoc) (not used in this project)
- [Validation API tutorial](https://www.baeldung.com/javax-validation-method-constraints)