
FROM bitnami/node:7.10.1-ol-7-r24 as development

FROM bitnami/oraclelinux-runtimes:7-r11
LABEL maintainer "Bitnami <containers@bitnami.com>"

COPY --from=development /opt/bitnami/node /opt/bitnami/node

ENV BITNAMI_APP_NAME="node" \
    BITNAMI_IMAGE_VERSION="7.10.1-ol-7-r24" \
    PATH="/opt/bitnami/node/bin:/opt/bitnami/python/bin:$PATH"

CMD ["node"]
