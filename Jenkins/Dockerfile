# Jenkins server with .Net build tools installed
FROM jenkins/jenkins:lts-alpine-jdk17
EXPOSE 8080
EXPOSE 50000
USER root

RUN addgroup jenkins root

# Install .Net and Docker
RUN apk -U add dotnet7-sdk docker docker-compose openssl

# Good idea to switch back to the jenkins user.
USER jenkins