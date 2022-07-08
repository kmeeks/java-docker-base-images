# Java build image
# TODO: Replace with FRB base image
FROM alpine:3.16.0

ARG JDK_INSTALLATION_VERSION=17.0.3_p7-r2
ARG JDK_PACKAGE=openjdk17
ARG MAVEN_VERSION=3.8.5-r0
ARG USER_HOME_DIR="/root"

RUN apk update && \
    apk add --no-cache ${JDK_PACKAGE}=${JDK_INSTALLATION_VERSION} maven=${MAVEN_VERSION}

ENV PATH="${PATH}:${JAVA_HOME}/bin"
ENV MAVEN_OPTS="-Xms512m -Xmx1056m"
ENV PATH="${PATH}:${M2}"