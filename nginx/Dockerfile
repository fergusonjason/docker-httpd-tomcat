FROM nginx:1.20.0

RUN mv /etc/nginx/conf.d/default.conf /etc/nginx/conf.d/default.conf.old
COPY nginx.conf /etc/nginx/conf.d/default.conf

EXPOSE 80