FROM ubuntu:22.04
RUN apt update && \
    apt install -y haproxy socat
COPY haproxy.cfg /usr/local/etc/haproxy/haproxy.cfg
CMD ["haproxy", "-f", "/usr/local/etc/haproxy/haproxy.cfg"]
