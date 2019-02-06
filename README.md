## OPENAPI 3.0

### Generating the APIs

[OpenAPI generator maven plugin](https://github.com/OpenAPITools/openapi-generator/blob/master/modules/openapi-generator-maven-plugin/README.md) is used to generate the API 
stubs.

The specification file is here:

`/northstar-controller/src/main/openapi/api.yaml`

Run 

```bash
mvn clean compile
``` 
to generate the APIs from the definitions in `api.yaml`. Run the application file
 
 `northstar-controller/target/generated-sources/openapi/src/main/java/org/openapitools/OpenAPI2SpringBoot.java`
 
 and the open [localhost:8081/swagger-ui.html](http://localhost:8081:swagger-ui.html) to see the results. 