# Upload Instructions

```
docker build --no-cache .
docker tag <id> diplodocusdb/alpine-diplodocusdb:latest
docker tag <id> diplodocusdb/alpine-diplodocusdb:<version>
docker login
docker push diplodocusdb/alpine-diplodocusdb:latest
docker push diplodocusdb/alpine-diplodocusdb:<version>
```
