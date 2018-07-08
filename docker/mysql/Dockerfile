FROM mysql:5.7

RUN apt-get update && apt-get install -y --no-install-recommends \
    vim \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN mv /etc/mysql/conf.d/mysql.cnf /etc/mysql/conf.d/mysql.cnf.orig
COPY mysql.cnf /etc/mysql/conf.d/
