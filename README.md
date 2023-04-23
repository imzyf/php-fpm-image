# My PHP-FPM Docker Base Image

- [GitHub php-fpm-image](https://github.com/imzyf/php-fpm-image/)
- [GitHub php-fpm-image - actions](https://github.com/imzyf/php-fpm-image/actions/)
- [DockerHub php-fpm - tags](https://hub.docker.com/repository/registry-1.docker.io/yifans/php-fpm/tags?page=1&ordering=last_updated)

## laradock/php-fpm Origin

- https://github.com/laradock/laradock/tree/master/php-fpm
- https://raw.githubusercontent.com/laradock/php-fpm/master/Dockerfile-7.1
- https://raw.githubusercontent.com/laradock/php-fpm/master/Dockerfile-7.4
- https://raw.githubusercontent.com/laradock/php-fpm/master/Dockerfile-8.1

```bash
docker run --rm --name=n81 yifans/php-fpm:main-nginx-8.1
docker build -f=Dockerfile-nginx-8.1 ./.
```

```bash
uname -a
cat /proc/version
cat /etc/issue
```

```
/etc/init.d/cron start
echo '* * * * * echo 22 >> /tmp/xxx.txt' > /etc/cron.d/crontab
```
