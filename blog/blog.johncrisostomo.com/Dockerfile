FROM johncrisostomo/ghost-on-docker-arm:0.11.4

ADD Vapor /var/www/ghost/content/themes/Vapor

RUN sed -i s/my-ghost-blog.com/blog.johncrisostomo.com/g config.js
