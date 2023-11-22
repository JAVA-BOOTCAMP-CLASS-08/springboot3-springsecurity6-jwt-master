# JWT Authentication and Authorization with Spring Boot 3 and Spring Security 6

Medium
Article: https://medium.com/@truongbui95/jwt-authentication-and-authorization-with-spring-boot-3-and-spring-security-6-2f90f9337421

```
curl --location --request POST 'http://localhost:8080/api/v1/auth/signup' \
--header 'Authorization: Basic YWRtaW46MTIzNA==' \
--header 'Content-Type: application/json' \
--data-raw '{
    "firstName" : "Andres",
    "lastName" : "Ramos",
    "email" : "andres.alberto.ramos@gmail.com",
    "password": "1234"
}'
```

```
curl --location --request POST 'http://localhost:8080/api/v1/auth/signin' \
--header 'Content-Type: application/json' \
--data-raw '{
    "email" : "andres.alberto.ramos@gmail.com",
    "password": "1234"
}'
```

```
curl --location --request GET 'http://localhost:8080/api/v1/resource' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJhbmRyZXMuYWxiZXJ0by5yYW1vc0BnbWFpbC5jb20iLCJpYXQiOjE3MDAyMTk5OTQsImV4cCI6MTcwMDIyMTQzNH0.L-2Hl0mvjTW-R04DDiFHN6pUIv2Lv1kiHH5StCRGHcU'
```
