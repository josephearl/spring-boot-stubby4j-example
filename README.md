# spring-boot-stubby4j-example

Run the tests with Spring Boot 2.3.3:

```
./mvnw -f pom.xml clean test
```

Results:

```
Tests run: 1, Failures: 0, Errors: 0, Skipped: 0
```

Run the tests with Spring Boot 2.3.4:

```
./mvnw -f pom-2.3.4.xml clean test
```

Results:

```
Tests in error: 
  shouldReturn200(org.example.CustomerControllerTest): org.yaml.snakeyaml.LoaderOptions.setMaxAliasesForCollections(I)V

Tests run: 1, Failures: 0, Errors: 1, Skipped: 0
```

Difference between the two POMs:

```
diff pom.xml pom-2.3.4.xml
```

Results:

```
20c20
<                 <version>2.3.3.RELEASE</version>
---
>                 <version>2.3.4.RELEASE</version>
```

