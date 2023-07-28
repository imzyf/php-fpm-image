# My PHP-FPM Docker Base Image

- [GitHub php-fpm-image](https://github.com/imzyf/php-fpm-image/)
- [GitHub php-fpm-image - actions](https://github.com/imzyf/php-fpm-image/actions/)
- [DockerHub php-fpm - tags](https://hub.docker.com/repository/registry-1.docker.io/yifans/php-fpm/tags?page=1&ordering=last_updated)

## laradock/php-fpm Origin

- <https://github.com/laradock/laradock/tree/master/php-fpm>
- <https://github.com/laradock/php-fpm>
- <https://raw.githubusercontent.com/laradock/php-fpm/master/Dockerfile-7.1>
- <https://raw.githubusercontent.com/laradock/php-fpm/master/Dockerfile-7.4>
- <https://raw.githubusercontent.com/laradock/php-fpm/master/Dockerfile-8.1>

```bash
docker build -f=Dockerfile-my-7.1 ./.

docker buildx build -f=Dockerfile-7.1 -t yifans/php-fpm:main-7.1 --platform=linux/arm64,linux/amd64 . --push
docker buildx build -f=Dockerfile-8.1 -t yifans/php-fpm:main-8.1 --platform=linux/arm64,linux/amd64 . --push


docker buildx build -f=Dockerfile-my-8.1 -t yifans/php-fpm:arm-my-8.1 . --push

docker buildx build -f=Dockerfile-7.1 -t yifans/php-fpm:arm-7.1 . --push
docker buildx build -f=Dockerfile-my-7.1 -t yifans/php-fpm:arm-my-7.1 . --push
```

## ARM

```bash
docker buildx build -f=Dockerfile-my-8.1 -t yifans/php-fpm:arm-my-8.1 . --push

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
