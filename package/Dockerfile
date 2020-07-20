FROM alpine:3.12

# Set Helm version
ENV DESIRED_VERSION=v3.2.3

RUN apk add --update bash ca-certificates openssl curl git \
    && (curl https://raw.githubusercontent.com/helm/helm/master/scripts/get | bash) \
    && helm version

COPY package.sh /usr/sbin/
