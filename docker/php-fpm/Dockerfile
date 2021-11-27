################################################################
##              Custom docker PHP container                   ##
## https://github.com/nigelritfeld/docker-development-network ##
################################################################

FROM php:8-fpm
# Downloading to install php extensions
ADD https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions /usr/local/bin/
# Running script to install PHP Extensions
RUN chmod +x /usr/local/bin/install-php-extensions && \
    install-php-extensions gd xdebug pdo_mysql mysqli zip bcmath
# Set timezone to your own prefrence
ENV TZ="Europe/Amsterdam"
# Added example development php.ini to make your own config
ADD php.ini /usr/local/etc/php

#############################################################################
## Only if you know what you're doing you can add your extra options below ##
#############################################################################
