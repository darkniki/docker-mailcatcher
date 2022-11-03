FROM alpine:3.16.2

MAINTAINER darkniki <darkniki777@gmail.com>

RUN apk add --no-cache --virtual .build-deps build-base sqlite-dev ruby-dev \
    && apk add --no-cache ruby sqlite-libs libstdc++ ruby-json ruby-etc \
    && gem install --no-document --platform ruby sqlite3 net-smtp mailcatcher  \
    && apk del .build-deps

EXPOSE 1025 1080

CMD ["mailcatcher", "--no-quit", "--foreground", "--ip=0.0.0.0"]
