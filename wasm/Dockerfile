# no apt to install jq, so we copy it over
# TODO: switch to cosmwasm/wasmd once it is published on dockerhub
FROM arkprotocol/wasmd:v0.53.0

USER root

RUN apk add --no-cache jq

WORKDIR /opt

COPY scripts/* /opt

CMD [ "/opt/run.sh" ]