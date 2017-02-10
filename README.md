# vertx
Vertx in Docker

Go to the [docker website](https://www.docker.com/products/overview) and install docker
Read the vertx documentation on [docker](https://hub.docker.com/r/vertx/vertx3-exec/)

Build the image with
```bash
docker build -t hello-world .
```

You can view new the docker image like this:
```
[vertx] docker images                                                                                                                                                                                                                        14:52:44  ☁  master ☂ ⚡
REPOSITORY                               TAG                 IMAGE ID            CREATED             SIZE
hello-world                              latest              97f227f3a664        5 months ago        194 MB
vertx/vertx3-exec                        latest              97f227f3a664        5 months ago        194 MB
```

```bash
docker run -i -t hello-world -version
```

```bash
npm install vertx3-full 
```

```bash
javac -cp ../../node_modules/vertx3-full/vertx/lib/vertx-core-3.3.3.jar:. Server.java
```


```bash
docker run -i -t -p 8080:8080 \
    -v $PWD:/verticles hello-world \
    run Server -cp /verticles/
```