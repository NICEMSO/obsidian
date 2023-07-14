

docker run -d -p 443:8443 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:18.0.0 start-dev --https-certificate-file=/root/server.crt.pem --https-certificate-key-file=/root/server.key.pem


docker run -d -p 443:8443 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:18.0.0 start-dev --https-certificate-file=/root/server.crt.pem --https-certificate-key-file=/root/server.key.pem


```
docker run -p 8443:8443 -e KEYCLOAK_ADMIN=admin  -e KEYCLOAK_ADMIN_PASSWORD=admin jboss/keycloak
```

```
docker run -p 8443:8443 -e KEYCLOAK_USER=username -e KEYCLOAK_PASSWORD=password jboss/keycloak
```



docker run -p 8443:8443 -p 8080:8080 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:20.0.2 start-dev


https://dkyou.tistory.com/54



![[Pasted image 20230111205922.png]]