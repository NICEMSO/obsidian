옥타아이덴티
https://youtu.be/MJ33pc34Usg
옥카 비교 
https://youtu.be/21MQozhb-SU
# Okta 및 스프링 부트를 사용한 SSO 데모
https://youtu.be/YpauXSVsbp8

![[Pasted image 20230114062649.png]]



![[Pasted image 20230114104253.png]]




JOSSO
https://hub.docker.com/r/atricore/josso

```
docker run \
        --name josso \
        --detach \
        --env JOSSO_CLIENT_ID="idbus-f2f7244e-bbcd-44ca-8b33-f5c0ade319f7" \
        --env JOSSO_CLIENT_SECRET="2oUHlv@HLT%vxK4G" \
        --env JOSSO_ADMIN_USR=myadmin \
        --env JOSSO_ADMIN_PWD=changeme \
        --env JOSSO_SKIP_ADMIN_CREATE=false \
        -p8081:8081 -p8101:8101 \
        atricore/josso-ce:2.6.0-3
```

```
docker run \
        --name iamtf \
        --detach \
        --env JOSSO_CLIENT_ID="idbus-f2f7244e-bbce-44ca-8b33-f5c0bde339f7" \
        --env JOSSO_CLIENT_SECRET="7oUHlv(HLT%vxK4L" \
        --env JOSSO_ADMIN_USR=myadmin \
        --env JOSSO_ADMIN_PWD=changeme \
        --env JOSSO_SKIP_ADMIN_CREATE=false \
        -p8081:8081 -p8101:8101 \
        atricore/iamtf:latest
```
