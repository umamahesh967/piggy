FROM java:8-jre
FROM maven
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

# Set the working directory to /app
WORKDIR /apigateway

# Copy the current directory contents into the container at /app
ADD . /apigateway

RUN mvn clean package

CMD ["mvn", "spring-boot:run"]

EXPOSE 4000
