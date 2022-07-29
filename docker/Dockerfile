FROM mongo:3.6

COPY docker-healthcheck /usr/local/bin/

# Useful Information:
# https://docs.docker.com/engine/reference/builder/#healthcheck
# https://docs.docker.com/compose/compose-file/#healthcheck
HEALTHCHECK --interval=30s --timeout=30s --start-period=0s --retries=3 \
CMD ["docker-healthcheck"]
