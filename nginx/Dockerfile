FROM ubuntu:latest

MAINTAINER sarvothaman vittal sarvothaman.vittal@gmail.com

RUN apt-get update && apt-get install nginx -y

#replace ngix default conf file
COPY default.conf /etc/nginx/conf.d/default.conf

# Make port 80 available for links and/or publish
EXPOSE 80

# Define working directory.
#WORKDIR /etc/nginx

CMD ["nginx","-g","daemon off;"]
