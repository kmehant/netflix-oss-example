# #
# # Dockerfile for Service C
# #

# FROM java:8



# # Install netcat
# # RUN apt-get update && apt-get install -y netcat

# VOLUME /tmp

# WORKDIR /service-c

# ADD target/service-c.jar service-c.jar

# RUN bash -c 'touch /service-c.jar'

# ADD run.sh run.sh
# RUN chmod 744 run.sh

# CMD ["./run.sh","service-c.jar"]

FROM openjdk:8
RUN apt-get update
RUN apt-get install -y curl


ADD ./target/service-c.jar service-c.jar

ENTRYPOINT ["java","-jar","/service-c.jar"]