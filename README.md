# example-service-gateway

# Service Gateway examples with Spring Boot
Example code of service gateway with Netflix Zuul. This gateway server configuration interfaces to **service discovery server** repository[https://github.com/superoutput/example-service-discovery](https://github.com/superoutput/example-service-discovery)

Check it out!

## Setup & Run
### Checkout **example-service-discovery** repository
1. Build and run App.java in *'service-discovery-server'*
2. Build and run App.java in *'service-discovery-client1'*
3. Build and run App.java in *'service-discovery-client2'*
4. Check student services by calling **HTTP GET** [http://localhost:8081/v1/student/61070003](http://localhost:8081/v1/student/61070003)
5. Get result from teacher service which pass request through student service by calling **HTTP GET** [http://localhost:8082/v1/teacher/studentReport](http://localhost:8082/v1/teacher/studentReport)

### Checkout this repository
1. Build and run App.java in *'service-gateway-server'*
2. Call **HTTP GET** [http://localhost:9090/studentservice/v1/student/61070003](http://localhost:9090/studentservice/v1/student/61070003)
3. Call **HTTP GET** [http://localhost:9090/teacherservice/v1/teacher/studentReport](http://localhost:9090/teacherservice/v1/teacher/studentReport)