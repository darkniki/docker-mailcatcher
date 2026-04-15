FROM alpine:3.23.3

LABEL maintainer="darkniki <darkniki777@gmail.com>"

RUN apk add --no-cache --virtual .build-deps build-base ruby-dev sqlite-dev \
    && apk add --no-cache ca-certificates libstdc++ ruby sqlite-libs \
    && gem install --no-document --platform ruby mailcatcher -v 0.10.0 \
    && apk del .build-deps

EXPOSE 1025 1080

CMD ["mailcatcher", "--no-quit", "--foreground", "--ip=0.0.0.0"]
