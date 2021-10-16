FROM litespeedtech/openlitespeed:1.6.9-lsphp74
LABEL createdby="Sashwat K <sashwat0001@gmail.com>"
LABEL maintainer="Sashwat K <sashwat0001@gmail.com>"

# Update and upgrade linux container
RUN apt-get -y update --fix-missing
RUN apt-get upgrade -y

# Install useful tools
RUN apt-get -y install apt-utils nano wget dialog

# Install important libraries
RUN apt-get -y install --fix-missing apt-utils build-essential git curl libcurl4-openssl-dev libzip-dev

# Copy files
COPY . /var/www/vhosts/localhost/html/