FROM ubuntu:latest

MAINTAINER Sarvo

RUN apt-get update && apt-get install nginx -y

COPY default.conf /etc/nginx/conf.d/default.conf

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
