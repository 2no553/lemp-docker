FROM mysql

RUN apt-get update && apt-get install -y --no-install-recommends \
    vim \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

COPY mysql.cnf /etc/mysql/conf.d/
