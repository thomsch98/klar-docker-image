FROM alpine

ADD https://github.com/optiopay/klar/releases/download/v2.0/klar-2.0-linux-amd64 /usr/bin/klar
ADD entrypoint.sh /

RUN apk add --update ca-certificates \
    && chmod a+x /usr/bin/klar entrypoint.sh

ENTRYPOINT [ "/entrypoint.sh" ]
