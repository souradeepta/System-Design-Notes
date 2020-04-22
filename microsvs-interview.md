## Microservices interview question and answers | Architecture design and Best practices

#### LINK:  https://www.youtube.com/watch?v=G0waumbpK48&t=0s

1. Microservice is the decoupling of application into smaller services to decouple services, make the system fault tolerant

2. For example for amazon you can separate the buyer and seller and admin

3.Monolothic is all in one. SOA has services inside an app with use of interfaces. Microservices are more segregated with for example separate auth layers for each micro service

4. Designing microservices is to understand users, how relationships are mapped and how are they dependent  and design databases accordingly

5. To change a monolith to microservices, change feature by feature to call external APIs of our new microservice

6. Advantages of microservices is Independent deployment and code change. Fault tolerant, scalable and no dependence on technologies

7. Disadvantages is individual strategies for each microservice and can have multiple layers of authentication for each microservice

8. If we have multiple layers of microservice we can put all logs to Splunk or Kibana/ES and for each request generate a correlation ID and it is passed to headers of the microservice. Health check can also help us log it

9. Dockerize your services and build the services seperately
10. All APIs are stateless because the ELB can direct any request to any micro service node. Hence state cannot be maintained. Sessions can be preserved on redis cache 

