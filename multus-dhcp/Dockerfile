FROM alpine:3.6
RUN apk add --update \
	curl \
  && curl -SLO https://github.com/containernetworking/plugins/releases/download/v0.8.7/cni-plugins-linux-arm64-v0.8.7.tgz \
  && tar xvfpz cni-plugins-linux-arm64-v0.8.7.tgz

ENTRYPOINT ["./dhcp", "daemon", "-hostprefix", "/host"]
