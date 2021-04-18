# Maven Getting started guide

https://maven.apache.org/guides/getting-started/index.html

## Setup

```
mvn -B archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4
```

## Workflow

```
mvn compile
mvn test

mvn package
java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App
```

## Old notes

```
to run tests:          mvn test
to run one test suite: mvn -Dtest=AppTest test
```
