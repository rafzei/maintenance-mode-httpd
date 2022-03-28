# Readme.md

## How to run maintenance mode

```sh
docker run -dit --name my-apache-app -p 80:80 -v "$PWD":/usr/local/apache2/htdocs/ -v "$PWD/conf/httpd.conf":/usr/local/apache2/conf/httpd.conf httpd:alpine3.15
```

### Check return code

```sh
curl http://localhost:80 -I
```
