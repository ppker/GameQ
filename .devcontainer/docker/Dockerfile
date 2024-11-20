# Define the DevContainer template to be used as the base
ARG TAG=8.2-bullseye
FROM mcr.microsoft.com/vscode/devcontainers/php:$TAG

# Update the registry once
RUN apt-get update

# Install ext-bz2
RUN apt-get install -y libbz2-dev \
    && docker-php-ext-configure bz2 \
    && docker-php-ext-install bz2