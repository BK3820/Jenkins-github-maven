# Springboot Hello World App
This repository is used for Jenkins Training Demo

### Build JAR (linux/macOS)
```
./mvnw clean package -DskipTests=true
```

### Build JAR (Windows)
```
mvnw clean package -DskipTests=true
```

### Unit Test Cases (linux/macOS)
```
./mvnw test
```

### Unit Test Cases (Windows)
```
mvnw test
```



- Total 6 test cases, out of which
  - 5 test cases will pass and 
  - 1 test case fails!
 
### Deploy/Run
```
java -jar target/hello-demo-*.jar 
```

### Integration Testing (Return 200 OK response)
```
curl -s http://localhost:6767/hello
```
