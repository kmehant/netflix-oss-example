# #
# # Dockerfile for Turbine
# #

# FROM java:8



# # Install netcat
# # RUN apt-get update && apt-get install -y netcat

# VOLUME /tmp

# WORKDIR /turbine

# ADD target/turbine.jar turbine.jar

# RUN bash -c 'touch /turbine.jar'

# ADD run.sh run.sh
# RUN chmod 744 run.sh

# EXPOSE 8989
# CMD ["./run.sh","turbine.jar"]

FROM openjdk:8
RUN apt-get update
RUN apt-get install -y curl


ADD ./target/turbine.jar turbine.jar

ENTRYPOINT ["java","-jar","/turbine.jar"]