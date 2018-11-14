# Dockerfile for lighttpd

FROM rocknsm/base:latest
MAINTAINER Bradford Dabbs <bndabbs@gmail.com>

RUN yum update -y; \
  yum install -y lighttpd; \
  rm -rf /var/cache/yum/*; \
  systemctl enable lighttpd

COPY conf/lighttpd.conf /etc/lighttpd/
COPY www/ /var/

EXPOSE 80/tcp
EXPOSE 443/tcp

CMD ["/usr/sbin/init"]
