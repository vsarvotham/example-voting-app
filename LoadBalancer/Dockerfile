FROM ubuntu:latest

MAINTAINER Sarvo

RUN apt-get update && apt-get install nginx -y

COPY index.html var/www/html/

COPY index.html /usr/share/nginx/html/index.html

RUN echo "$(hostname -I)" >> var/www/html/index.html

RUN echo "$(hostname -I)" >> /usr/share/nginx/html/index.html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
