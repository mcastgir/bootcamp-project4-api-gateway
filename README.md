# Project Api Gateway
> Microservice **Api Gateway** Bootcamp NTT Data

This project include:
- Spring Cloud Config
- Spring Cloud Gateway
- Spring Cloud Eureka Client
- Spring Cloud Bootstrap
- Github Actions
- Docker

### Docker

1. Create Image Config Server in Docker
```  
docker build -t api-gateway .
```

2. Create Container

```
docker run -p 8090:8090 --name api-gateway-instance --link config-server-instance:latest -d api-gateway:latest
```