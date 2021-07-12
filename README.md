### Simple lemp stack from laradock
This is basic lemp stack using docker-compose was created by laradock
Using certbot to autogenerate let's encrypt ssl and support autorenew 
Reference: https://pentacent.medium.com/nginx-and-lets-encrypt-with-docker-in-less-than-5-minutes-b4b8a60d3a71

#### How to use:
1. docker-compose up -d 
2. Change domain name in init-letsencrypt.sh in line 8
3. Config ssl in nginx config file. Using private key in folder /etc/letsencrypt