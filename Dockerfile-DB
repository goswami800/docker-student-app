FROM mysql:latest

LABEL database="studentapp"

# Environment variables for MySQL image
ENV MYSQL_ROOT_PASSWORD=admin1234 \
    MYSQL_USER=admin \
    MYSQL_PASSWORD=admin1234 \
    MYSQL_DATABASE=studentapp

# Initialization script
COPY init-db.sql /docker-entrypoint-initdb.d/

# Expose MySQL port
EXPOSE 3306

# Start the MySQL server (handled by base image)
CMD ["mysqld"]
