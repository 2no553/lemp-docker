FROM nginx

RUN apt-get update && apt-get install -y --no-install-recommends \
    net-tools \
    vim \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN mv /etc/nginx/conf.d/default.conf /etc/nginx/conf.d/default.conf.orig

COPY default.conf /etc/nginx/conf.d/
