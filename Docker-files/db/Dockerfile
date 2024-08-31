#Dockerfile for mysql 

FROM mysql:8.0.33
LABEL "Project"="Vprofile"
LABEL "Author"="Brian"
RUN groupadd -r mysql && useradd -r -g mysql mysql
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
ENV MYSQL_ROOT_PASSWORD="password"
ENV MYSQL_DATABASE="accounts"

ADD db_backup.sql /docker-entrypoint-initdb.d
