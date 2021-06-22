**Definition**

Web applications typically runs on servers were we are limitied to resources in terms of RAM,CPU and network bandwith. In absence of rate limiting the servers cannot limit the number of call to an endpoint. Every request consumes some part of all the above mentioned resources which when uncontrolled leads to oveuse of resouces and application failure. Some examples of attacks.
- Non authencated api : As our endpoints are exposed an attacker can use the endpoint programetically call the endpoint to simulate some around 10's million calls per second as result server down.
- Decrease server performance : A user of a system for example excel uploading some data he can again run a bot and increase processing elements for the api and hence leading to slow performance

**Purpose**
- Adding an added security layer for infrastructure

**Benefits**
- DDOS attack leading to resource problems of servers
- Limiting the number of call that can be done to a particular end point

**Methods**
- Restrict number of api calls that can be made to an api endpoint using algorithms like leaky bucket , sliding window.

**Current focus**
- Limiting a number of call in open api
- Limit/Track number of calls on an enpoint by a particular user

**Approach example**
- [Node](https://www.npmjs.com/package/express-rate-limit) 
- [Spring Boot](https://www.baeldung.com/spring-bucket4j) 

**Todo**

- [ ] Rate limiting at IP level

