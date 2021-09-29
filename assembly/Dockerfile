FROM ubuntu:latest
ARG DEBIAN_FRONTEND=noninteractive
RUN apt update && apt install default-jdk git maven -y
# && git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp/hello \
# && mvn -q -f /tmp/hello package
VOLUME [ "/source" ]
CMD ["git", "clone", "https://github.com/boxfuse/boxfuse-sample-java-war-hello.git", \
    "/source", ";", "mvn", "-q", "-f", "/source", "package"]