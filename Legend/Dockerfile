FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
x11-apps \
xauth \
openjdk-17-jre \
&& rm -rf /var/lib/apt/lists/*

COPY calc.jar /app/calc.jar

ENV DISPLAY=host.docker.internal:0

CMD ["java", "-jar", "/app/calc.jar"]
