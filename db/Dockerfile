FROM guacamole/guacamole AS schema
RUN /opt/guacamole/bin/initdb.sh --postgres > /opt/initdb.sql

FROM postgres:11.2-alpine
COPY --from=schema /opt/initdb.sql /docker-entrypoint-initdb.d
