# London-API

An API, built with Maven and Spring Boot, that calls https://bpdts-test-app.herokuapp.com/ and returns people who are listed as either living in London, or whose current coordinates are within 50 miles of London.


## Requests

The API supports the following requests:

Request | Path | Returns
--------|------|--------
`GET`|`/London`| a JSON-formatted list of users who are listed as living in London.
`GET`|`/FiftyMiles` | a JSON-formatted list of users whose current coordinates are within 50 miles of London.
`GET`|`/LondonOrFiftyMiles` | a JSON-formatted list resulting from the combination of the two requests above.

## Running the application
After downloading the files, the application can be run from the command line with Maven as follows:

`./mvnw spring-boot:run`

The service will then run on your machine at `http://localhost:8000`, and `GET` requests wil be  accessible from the following URLs:

- //localhost:8000/London
- //localhost:8000/FiftyMiles
- //localhost:8000/LondonOrFiftyMiles



