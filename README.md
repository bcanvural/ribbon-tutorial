# Ribbon, Client Side LoadBalancer

https://spring.io/guides/gs/client-side-load-balancing/

Run 3 instances of say-hello service:

In /say-hello
```bash
SERVER_PORT=8888 mvn spring-boot:run
SERVER_PORT=8090 mvn spring-boot:run
SERVER_PORT=9092 mvn spring-boot:run
```
Run user service:

In /user

```bash
mvn spring-boot:run
```

Then:

```bash
curl localhost:8888/hi
```


