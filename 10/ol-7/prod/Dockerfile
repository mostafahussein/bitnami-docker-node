
FROM bitnami/node:10.6.0-ol-7-r9 as development

FROM bitnami/oraclelinux-runtimes:7-r11
LABEL maintainer "Bitnami <containers@bitnami.com>"

COPY --from=development /opt/bitnami/node /opt/bitnami/node

ENV BITNAMI_APP_NAME="node" \
    BITNAMI_IMAGE_VERSION="10.6.0-ol-7-r9" \
    PATH="/opt/bitnami/node/bin:/opt/bitnami/python/bin:$PATH"

CMD ["node"]
