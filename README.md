# testHystrixService
Part of a spring cloud sample. Tutorial link : https://www.youtube.com/watch?v=ZyK5QrKCbwM

## Hystrix Service
Hystrix allows to monitor the app 

Hystrix is a library that helps you control the interactions between these distributed services by adding latency tolerance and fault tolerance logic.

## Requirements 

- Spring Boot
- Java 8
- Config server from :https://github.com/EstefaniaAR/testConfigServer.git
- Reservation service from: https://github.com/EstefaniaAR/testReservationService.git
- Eureka Service: https://github.com/EstefaniaAR/testEurekaService.git
- Discovery Service: https://github.com/EstefaniaAR/testDiscoveryService.git
- Reservation Client: https://github.com/EstefaniaAR/testReservationClient.git

## Dependencies
      <dependencies>
        <dependency>
          <groupId>org.springframework.cloud</groupId>
          <artifactId>spring-cloud-starter-config</artifactId>
        </dependency>
        <dependency>
          <groupId>org.springframework.cloud</groupId>
          <artifactId>spring-cloud-starter-netflix-hystrix-dashboard</artifactId>
        </dependency>

        <dependency>
          <groupId>org.springframework.boot</groupId>
          <artifactId>spring-boot-starter-test</artifactId>
          <scope>test</scope>
        </dependency>
        <dependency>
              <groupId>org.springframework.boot</groupId>
              <artifactId>spring-boot-starter-actuator</artifactId>
          </dependency>
       </dependencies>
## Run
Run the main clas as Spring boot application

## Query
Display dashboard

 - http://localhost:8010/hystrix
 - localhost:9999/actuator/hystrix.stream on text box and click on monitor stream
 - Generate data flow by requesting http://localhost:9999/reservations/names 
 

