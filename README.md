# nginx-master
In this Nginx, I build a Node.js webserver and set up dockerized instances. We then configure Nginx as a reverse proxy to load balance traffic to those backend servers and finally we configure a secure HTTPS connection to the Nginx proxy with a self-signed TLS certificate.

# To Run

docker compose up --build -d

In nginx.conf file update the config and run

--> nginx

To generate certificates
--> openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout nginx-selfsigned.key -out nginx-selfsigned.crt