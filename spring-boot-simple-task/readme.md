# Simple Spring Task

Run `com.container.spring.simple.task.SpringSimpleTaskApplication` as a Java Application.

Runs `com.container.spring.simple.task.TaskImpl.performTask()` at launch

### Creating Containers

- mvn clean package

```
docker login
docker push @@REPO@@/aws-simple-spring-task:1.0.0-RELEASE
```
- docker run mibrahimdocker/aws-simple-spring-task:1.0.0-RELEASE