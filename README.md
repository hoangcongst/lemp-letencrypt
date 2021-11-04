### Simple lemp stack from laradock
This is basic lemp stack using docker-compose was created by laradock
Using certbot to autogenerate let's encrypt ssl and support autorenew 
Reference: https://pentacent.medium.com/nginx-and-lets-encrypt-with-docker-in-less-than-5-minutes-b4b8a60d3a71

#### How to use:
1. docker-compose up -d nginx certbot
3. Config ssl in nginx config file. Using private key in folder /etc/letsencrypt

**Adding into conf files**
```
ssl_certificate /etc/letsencrypt/live/example.org/fullchain.pem;
ssl_certificate_key /etc/letsencrypt/live/example.org/privkey.pem;
include /etc/letsencrypt/options-ssl-nginx.conf;
ssl_dhparam /etc/letsencrypt/ssl-dhparams.pem;
```
