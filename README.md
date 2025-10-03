# hello-java-maven

A simple **Java HelloWorld application** built with **Maven**, intended to be used with a **Jenkins Freestyle job**.  
This repo demonstrates a minimal CI build: `mvn clean package` â†’ `BUILD SUCCESS`.

---

## Project structure

```
hello-java-maven/
 - pom.xml
 - src/
     - main/
         - java/
             - HelloWorld.java
```

---
##  Build with Maven

From the project root run:
```bash
mvn clean package
```

After a successful build, the JAR will be produced at:
```
target/hello-1.0.jar
```

Expected Maven snippet in console:
```
[INFO] BUILD SUCCESS
```

---

## Run the application

Because `HelloWorld` is in the default package, you can run:

```bash
java -cp target/hello-1.0.jar HelloWorld
```

Expected output:
```
Hello, Jenkins + Maven!
```
