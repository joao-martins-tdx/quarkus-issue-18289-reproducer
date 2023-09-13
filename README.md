# Quarkus issue 18289 reproducer

Reproducer project for https://github.com/quarkusio/quarkus/issues/18289.

## Pre-requisites

* JDK 17+ installed with JAVA_HOME configured appropriately
* Apache Maven 3.9.3

## Steps to reproduce

1. Clone the repository: `git clone https://github.com/joao-martins-tdx/quarkus-issue-18289-reproducer.git`
2. Run GreetingResourceTest#testHelloEndpoint: `mvn test`

## Expected behaviour

The test sends the request to http://localhost:8081/api/v1/hello and succeeds.

## Actual behaviour

The test sends the request to http://localhost:8081/hello and fails with a `404 Not Found` error.
