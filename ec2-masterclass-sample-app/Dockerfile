From openjdk:8


HEALTHCHECK --interval=5s \
            --timeout=5s \
            CMD curl -f http://127.0.0.1:4567 || exit 1

EXPOSE 4567
