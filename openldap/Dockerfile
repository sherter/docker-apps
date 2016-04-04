FROM alpine:3.3

RUN apk add --no-cache openldap openldap-clients

VOLUME /var/lib/openldap

ENTRYPOINT ["slapd"]

EXPOSE 389
# slapd runs in foreground if a debug level is set
CMD ["-d0"]
