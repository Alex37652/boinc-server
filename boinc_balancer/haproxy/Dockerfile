FROM haproxy:1.8.30

RUN groupadd -f haproxy && useradd -g haproxy haproxy; exit 0
RUN mkdir -p /var/lib/haproxy
RUN mkdir -p /run/haproxy/
RUN mkdir -p /dev/log
USER haproxy

COPY haproxy.cfg /usr/local/etc/haproxy/haproxy.cfg

EXPOSE 80
