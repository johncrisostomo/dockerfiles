FROM resin/rpi-raspbian:latest

RUN apt-get update && apt-get install -qy nginx

ADD index.html /var/www/html/

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
