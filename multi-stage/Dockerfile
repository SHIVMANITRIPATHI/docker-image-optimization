FROM eclipse-temurin:17-jdk AS build

WORKDIR /app
COPY Test.java .

RUN javac Test.java
FROM eclipse-temurin:17-jre

WORKDIR /app
COPY --from=build /app/Test.class .

CMD ["java", "Test"]
