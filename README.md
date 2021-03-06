# Docker Images
Some Dockerfile

# PHP 7.2、7.3、7.4
DockerHub: https://hub.docker.com/r/coderking/php
## Base
Feature
- Install Composer
- Install redis, gd, pdo_mysql, zip and exif extensions

Pull image
```bash
docker pull coderking/php:7.2
docker pull coderking/php:7.3
docker pull coderking/php:7.4
```

## Local
Feature
- Extends Base
- Install xdebug extensions
- Add `post_max_size=20M` and `upload_max_filesize=20M` to php.ini

Pull image
```bash
docker pull coderking/php:7.2-local
docker pull coderking/php:7.3-local
docker pull coderking/php:7.4-local
```

## Production
Feature
- Extends Base
- Install opcache extensions
- Add `post_max_size=20M` and `upload_max_filesize=20M` to php.ini

Pull image
```bash
docker pull coderking/php:7.2-production
docker pull coderking/php:7.3-production
docker pull coderking/php:7.4-production
```

# MySQL 8.0
DockerHub: https://hub.docker.com/r/coderking/mysql
## Local
Feature
- Add `default-authentication-plugin=mysql_native_password` and `bind-address=0.0.0.0` to my.cnf

Pull image
```bash
docker pull coderking/mysql:8.0-local
```

## Production
Feature
- Add `default-authentication-plugin=mysql_native_password` to my.cnf

Pull image
```bash
docker pull coderking/mysql:8.0-production
```
# MySQL Client
DockerHub: https://hub.docker.com/r/coderking/mysql-client

Pull image
```bash
docker pull coderking/mysql-client:1.0
```

# NGINX 1.7
DockerHub: https://hub.docker.com/r/coderking/nginx

Feature
- Add [nginx.conf](./nginx/1.7/conf/nginx.conf)
- Remove /etc/nginx/conf.d/default.conf

Pull image
```bash
docker pull coderking/nginx:1.7
```

# Elasticsearch 7.4、7.6
DockerHub: https://hub.docker.com/r/coderking/elasticsearch

Feature
- Install elasticsearch-analysis-ik

Pull image
```bash
docker pull coderking/elasticsearch:7.4
docker pull coderking/elasticsearch:7.6
```
