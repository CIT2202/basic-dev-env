FROM mcr.microsoft.com/devcontainers/php:8.3

# MariaDB client (for the `mysql` command) and PHP database drivers
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get install -y --no-install-recommends mariadb-client \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/*

RUN docker-php-ext-install mysqli pdo pdo_mysql

