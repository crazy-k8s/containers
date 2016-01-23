FROM golang
MAINTAINER jono <_@oj.io> (@onojw)

RUN set -eux &&\
  go get github.com/skynetservices/skydns &&\
  go install github.com/skynetservices/skydns

EXPOSE 53 53/udp
ENTRYPOINT ["/go/bin/skydns"]
