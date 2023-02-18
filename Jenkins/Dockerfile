# Jenkins server with .Net build tools installed
FROM jenkins/jenkins:lts-alpine-jdk17
EXPOSE 8080
EXPOSE 50000
USER root

# Install .Net
RUN apk -U add dotnet7-sdk

# Good idea to switch back to the jenkins user.
USER jenkins