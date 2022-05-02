FROM debian:10

RUN apt-get update && apt install -y php-curl php-fpm php-mbstring php-mysql && rm -rf /var/lib/apt/*

VOLUME /var/run/php

CMD ["/usr/sbin/php-fpm7.3", "--nodaemonize", "--fpm-config", "/etc/php/7.3/fpm/php-fpm.conf"]
