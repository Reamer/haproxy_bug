FROM haproxy:2.4.19-bullseye
USER root
RUN apt update && \
    apt install -y socat
COPY haproxy.cfg /usr/local/etc/haproxy/haproxy.cfg
CMD ["haproxy", "-f", "/usr/local/etc/haproxy/haproxy.cfg"]
