# #
# # Dockerfile for Service C
# #

# FROM java:8



# # Install netcat
# # RUN apt-get update && apt-get install -y netcat

# VOLUME /tmp

# WORKDIR /client-traffic-generator

# ADD target/client-traffic-generator.jar client-traffic-generator.jar

# RUN bash -c 'touch /client-traffic-generator.jar'

# ADD run.sh run.sh
# RUN chmod 744 run.sh

# CMD ["./run.sh","client-traffic-generator.jar"]


FROM openjdk:8
RUN apt-get update
RUN apt-get install -y curl


ADD ./target/client-traffic-generator.jar client-traffic-generator.jar

ENTRYPOINT ["java","-jar","/client-traffic-generator.jar"]
