## lemp-docker

### version info
- Mac OS 10.11.6（El Capitan）
- Docker Toolbox
  - Docker version 18.03.0-ce
  - Oracle VM VirtualBox Manager 5.2.12
- nginx version: nginx/1.15.1
- PHP 7.2.7 (fpm-fcgi)
- mysql  Ver 14.14 Distrib 5.7.22
- phpMyAdmin 4.8.2

### directory map

```
.
├── README.md
├── data
│   ├── mysql
│   └── public
│       └── index.php
└── docker
    ├── docker-compose.yml
    ├── logs
    │   └── nginx
    ├── mysql
    │   ├── Dockerfile
    │   ├── docker-entrypoint-initdb.d
    │   └── mysql.cnf
    ├── nginx
    │   ├── Dockerfile
    │   ├── default.conf
    │   └── sites
    └── php-fpm
        ├── dockerfile
        └── www.conf
```

### getting started

```
$ git clone https://github.com/2no553/lemp-docker.git
$ cd lemp-docker/docker/
$ docker-compose up -d --build
```
