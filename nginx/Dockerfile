FROM ubuntu:latest

MAINTAINER sarvothaman vittal sarvothaman.vittal@gmail.com

RUN apt-get update && apt-get install nginx -y

RUN rm /etc/nginx/sites-available/default
#replace ngix default conf file
COPY default.conf /etc/nginx/sites-enabled/default

# Make port 80 available for links and/or publish
EXPOSE 80

# Define working directory.
#WORKDIR /etc/nginx

CMD ["nginx","-g","daemon off;"]
