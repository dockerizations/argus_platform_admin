# Argus Platform Admin

This repository contains Dockerfile of `sail-8.3/app` for Docker's build
published to the public [Docker Hub Registry][docker-hub-registry].

## Run environment

```shell
$ # docker system prune -a
$ cd ~
$ cd /path/to/projects/dockerizations/argus_platform_admin/
$ ./vendor/bin/sail build --no-cache
$ ./vendor/bin/sail up -d
$ ./vendor/bin/sail bash
$ ./vendor/bin/sail down
$ exit
```

### Run custom local environment (example)

```shell
$ # docker system prune -a
$ cd ~
$ cd /path/to/projects/dockerizations/argus_platform_admin/
$ ./vendor/bin/sail -f ./docker-compose-dev.yml build --no-cache
$ ./vendor/bin/sail -f ./docker-compose-dev.yml up -d
$ ./vendor/bin/sail bash
$ ./vendor/bin/sail -f ./docker-compose-dev.yml down
$ exit
```

## Credits

- [Nikola Zeravcic][link-author]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more
information.

[docker-hub-registry]: https://hub.docker.com/
[link-author]: https://github.com/zeravcic
