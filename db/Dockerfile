FROM mysql:latest

COPY ./init/init.sql /docker-entrypoint-initdb.d/init.sql

ENV POSTGRES_USER postgres
ENV POSTGRES_PASSWORD postgres

EXPOSE 5432