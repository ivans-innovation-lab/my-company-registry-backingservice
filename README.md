# [projects](http://ivans-innovation-lab.github.io/projects)/my-company-registry-backingservice [![CircleCI](https://circleci.com/gh/ivans-innovation-lab/my-company-registry-backingservice.svg?style=svg)](https://circleci.com/gh/ivans-innovation-lab/my-company-registry-backingservice)
Netflix Eureka is a service registry. It provides a REST API for service instance registration management and for querying available instances. Netflix Ribbon is an IPC client that works with Eureka to load balance(client side) requests across the available service instances.

## Running instructions

Make sure that services are running:

 - [my-company-configuration-backingservice](https://github.com/ivans-innovation-lab/my-company-configuration-backingservice)

```bash
$ cd my-company-registry-backingservice
$ ./mvnw spring-boot:run
```

Application will be available on port 8761 (http://localhost:8761)
