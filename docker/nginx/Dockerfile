FROM debian:10

RUN apt update && apt install -y nginx-full libnginx-mod-http-lua && rm -rf /var/lib/apt/*

CMD ["/usr/sbin/nginx", "-g", "daemon off; master_process on;"]
