FROM alpine:latest

WORKDIR /app

COPY script.sh /app/script.sh

RUN chmod +x /app/script.sh

ENTRYPOINT ["/app/script.sh"]

CMD ["User-default"]