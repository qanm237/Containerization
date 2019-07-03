FROM ubuntu:16.04
RUN apt-get update -y
RUN apt-get install nginx -y
RUN rm /usr/share/nginx/html/index.html
COPY .  /var/www/html/
RUN service nginx start
EXPOSE 80
CMD ["nginx","-g","daemon off;"]
