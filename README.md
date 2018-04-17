# My Docker PHP-FPM

搭建一套自己的开发环境 之 PHP-FPM。

## Build configurations

| Source Type | Source | Docker Tag | Dockerfile location |
| --- | --- | --- | --- |
| Branch | master | release-7.1 | Dockerfile-7.1 |
| Branch | master | release-5.6 | Dockerfile-5.6 |
| Tag | /^v([0-9.]+)$/ | 7.1-{\1} | Dockerfile-7.1 |
| Tag | /^v([0-9.]+)$/ | 5.6-{\1} | Dockerfile-5.6 |

> Reference:
> - [laradock/laradock](https://github.com/laradock/laradock)
