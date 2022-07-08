# Java build image
# TODO: Replace with FRB base image
FROM alpine:3.16.0

ARG JRE_INSTALLATION_VERSION=17.0.3_p7-r2
ARG JRE_PACKAGE=openjdk17-jre
ARG USER_HOME_DIR="/root"

RUN apk update && \
    apk add --no-cache ${JRE_PACKAGE}=${JRE_INSTALLATION_VERSION}

ENV PATH="${PATH}:${JAVA_HOME}/bin"