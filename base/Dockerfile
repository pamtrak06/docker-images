FROM armhf/alpine:3.5 as base
RUN apk --no-cache --update upgrade && apk --no-cache add ca-certificates

FROM scratch
COPY --from=base /etc/ssl/certs/ca-certificates.crt /etc/ssl/certs/ca-certificates.crt
