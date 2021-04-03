# GCC with DiplodocusDB Docker Images

Configuration files for [Docker](https://www.docker.com/) images that contain [GCC](https://gcc.gnu.org/) and
the DiplodocusDB components. As the DiplodocusDB components rely heavily on Ishiko/C++ framework it is also
part of the images.

The images are available from [Docker Hub](https://hub.docker.com/r/diplodocusdb/gcc-diplodocusdb).

# Image Contents

The images are based on the [the official GCC Docker image](https://hub.docker.com/_/gcc).

# Upload Instructions

```
docker build --no-cache .
docker tag <id> diplodocusdb/gcc-diplodocusdb:latest
docker tag <id> diplodocusdb/gcc-diplodocusdb:<version>
docker login
docker push diplodocusdb/gcc-diplodocusdb:latest
docker push diplodocusdb/gcc-diplodocusdb:<version>
```
