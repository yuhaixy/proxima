FROM alpine:latest

RUN apk --no-cache add dnsmasq

RUN echo "conf-dir=/etc/dnsmasq.d" >> /etc/dnsmasq.conf

EXPOSE 53 53/udp

VOLUME /etc/dnsmasq.d

ENTRYPOINT ["dnsmasq", "-k"]