# #
# # Dockerfile for Service B
# #

# FROM java:8



# # Install netcat
# # RUN apt-get update && apt-get install -y netcat

# VOLUME /tmp

# WORKDIR /service-a

# ADD target/service-a.jar service-a.jar

# RUN bash -c 'touch /service-a.jar'

# # ADD run.sh run.sh
# # RUN chmod 744 run.sh

# # CMD ["./run.sh","service-a.jar"]


FROM openjdk:8
RUN apt-get update
RUN apt-get install -y curl


ADD ./target/service-a.jar service-a.jar

ENTRYPOINT ["java","-jar","/service-a.jar"]