# no apt to install jq, so we copy it over
FROM cosmwasm/wasmd:v0.52.0

USER root

RUN apk add --no-cache jq

WORKDIR /opt

COPY scripts/* /opt

CMD [ "/opt/run.sh" ]