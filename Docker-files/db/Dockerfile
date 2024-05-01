FROM mysql:8.0.33
LABEL "Project"="Vprofile"
LABEL "Author"="BoBo"

ENV MYSQL_ROOT_PASSWORD="vprodbpass"
ENV MYSQL_DATABASE="accounts"

ADD db_backup.sql docker-entrypoint-initdb.d/db_backup.sql
RUN rm -rf /var/lib/mysql/*
## we can expose port 3306 but that's taken care by the MySQL image at the beginning

EXPOSE 3306
