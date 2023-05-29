FROM nginx

COPY reverse-proxy-template /etc/nginx/conf.d/reverse-proxy.conf

COPY certs/fullchain.pem /etc/nginx/TLS/fullchain.pem
COPY certs/fullchain1.pem /etc/nginx/TLS/fullchain1.pem
COPY certs/privkey.pem /etc/nginx/TLS/privkey.pem
COPY certs/privkey1.pem /etc/nginx/TLS/privkey1.pem

EXPOSE 80
EXPOSE 443
