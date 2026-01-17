FROM ubuntu:latest

WORKDIR /app

COPY . .

RUN apt update -y && \
    apt install openjdk-17-jdk -y && \
    javac Test.java

CMD ["java", "Test"]
