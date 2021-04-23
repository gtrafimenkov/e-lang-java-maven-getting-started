# Maven Getting started guide

- https://maven.apache.org/guides/getting-started/index.html
- plus maven-jar-plugin configured to add the main class
- plus JaCoCo library is configured to generate unit tests coverage

## Setup

```
mvn -B archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4
```

## Workflow

```
mvn compile
mvn test

mvn package
java -jar target/my-app-1.0-SNAPSHOT.jar

# for the case when the main class is not specified
# in the jar's manifest
java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App
```

## Unit tests coverage report

- `mvn jacoco:prepare-agent verify jacoco:report`
- check ./target/site/jacoco/index.html

## Old notes

```
to run tests:          mvn test
to run one test suite: mvn -Dtest=AppTest test
```
