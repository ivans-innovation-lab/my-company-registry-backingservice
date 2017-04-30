# my-company-registry-backingservice
Netflix Eureka is a service registry. It provides a REST API for service instance registration management and for querying available instances. Netflix Ribbon is an IPC client that works with Eureka to load balance(client side) requests across the available service instances.

## Running instructions

```bash
$ cd my-company-configuration-backingservice
$ ./mvnw spring-boot:run
```

Application will be available on port 8761 (http://localhost:8761)
