FROM alpine:latest

RUN addgroup -S appgroup && adduser -S appuser -G appgroup \
    && apk --no-cache add shadow \
    && usermod -u 1000  appuser \
    && groupmod -g 1000 appgroup \
    && touch /home/test \
    && chown appuser:appgroup /home/test

VOLUME /home
