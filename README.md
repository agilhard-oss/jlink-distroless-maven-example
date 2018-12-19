# jlink-distroless-maven-example

This project shows how you can build a tiny Docker image based on the google [distroless](https://github.com/GoogleContainerTools/distroless) docker base image with a custom modular Java run-time image for your app.

This example is using the [link-jpackager-maven-plugin](https://github.com/agilhard-oss/jlink-jpackager-maven-plugin).

The [link-jpackager-maven-plugin](https://github.com/agilhard-oss/jlink-jpackager-maven-plugin) is not (yet?) available on maven central you must download
and compile and install that to your maven Repository before you can use
this example.

For a similar example using the [maven-jlink-plugin](https://github.com/apache/maven-jlink-plugin) look at
[https://github.com/bei/maven-jlink-distroless-example](https://github.com/bei/maven-jlink-distroless-example).


After building the docker image you can start it with

```
docker run agilhard/jlink-distroless-example
```

## Prerequisites

- [JDK](http://jdk.java.net/)
- [Maven](https://maven.apache.org/)
- [Docker](https://www.docker.com/)

**You will need at least Java 9:** This project uses [jlink](https://docs.oracle.com/javase/9/tools/jlink.htm) to assemble modules and their dependencies into a custom Java run-time image.



