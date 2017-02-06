FROM resin/rpi-raspbian:latest

RUN apt-get update && apt-get install -qy nginx

WORKDIR /etc/nginx/ 

RUN rm /var/www/html/index.nginx-debian.html && \
    rm sites-available/default && \
    rm sites-enabled/default && \
    rm nginx.conf

COPY nginx.conf /etc/nginx/

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
