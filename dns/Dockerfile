FROM alpine:3
RUN apk add --no-cache dnsmasq
CMD ["dnsmasq", "--keep-in-foreground", "--no-resolv", "--no-hosts", "--address=/case.test/192.0.2.10"]