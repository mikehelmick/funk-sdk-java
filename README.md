# funk-java-go
fun(k) SDK in Java

# demo version

Currently requires that your project lives in

# others

```
kn funk init java
kn funk function create HelloWorld --t com.mikehelmick.eventutils.user.user
mvn package
mvn dependency:copy -Dartifact='com.google.cloud.functions.invoker:java-function-invoker:1.0.0-alpha-2-rc3' -DoutputDirectory=.
mvn package
java -jar java-function-invoker-1.0.0-alpha-2-rc3.jar --classpath target/funk-1.0-SNAPSHOT-jar-with-dependencies.jar --target com.example.funks.HelloWorld   
```
