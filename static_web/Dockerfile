FROM nginx

ADD static.zip /tmp

RUN apt update \
    && apt -y install unzip \
    && unzip -d /tmp /tmp/static.zip \
    && mv /tmp/static /usr/share/nginx/html/companyNews \
    && rm /tmp/static.zip

COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 80
