# Hello World Rest API

- Main class com.container.rest.webservices.restfulwebservices.RestfulWebServicesApplication 
- You cannot run this app on local as it is configured to run on port 80 - https://serverfault.com/questions/112795/how-to-run-a-server-on-port-80-as-a-normal-user-on-linux. You can run it as a docker container as shown below


### Creating Containers

- mvn clean package

```
docker login
docker push @@REPO@@/aws-hello-world-rest-api:1.0.0-RELEASE
```
- docker run --publish 8200:80 mibrahimdocker/aws-hello-world-rest-api:1.0.0-RELEASE

## Test URLs

- http://localhost:8200/hello-world

```txt
Hello World
```

- http://localhost:8200/hello-world-bean

```json
{"message":"Hello World - Changed"}
```

- http://localhost:8200/hello-world/path-variable/mibrahimdocker

```json
{"message":"Hello World, mibrahimdocker"}
```

