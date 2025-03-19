FROM ubuntu:24.04

RUN apt-get update && apt-get install -y unbound syslog-ng

COPY unbound.conf /etc/unbound/unbound.conf

CMD ["sh", "-c", "unbound -c /etc/unbound/unbound.conf & syslog-ng -f /etc/syslog-ng/syslog-ng.conf & sleep infinity"]