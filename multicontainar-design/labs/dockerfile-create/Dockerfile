FROM ubi7/ubi:7.7

MAINTAINER shin553 <v21xsy3c@rc5.so-net.ne.jp>

LABEL description="A basic Apache container on RHEL 7 UBI"

RUN yum install -y httpd && \
    yum clean all

RUN echo "Hello from Dockerfile" > /usr/share/httpd/noindex/index.html

EXPOSE 80

ENTRYPOINT  ["httpd", "-D", "FOREGROUND"]

