# laravel-docker

Added files/folders in this Laravel-repo from original laravel/laravel 5.8:
* docker-compose.yaml
* config/docker/*

And .gitignore has these two lines added to disable checking in mysql-data and elasticsearch-data:
```
.data
.esdata
```

## Hosts
Please, rember to register `local.laravel-docker.se` in your local hosts, eg: /etc/hosts as:
```
    # /etc/hosts
    127.0.0.1 local.laravel-docker.se
```

## Examples
* Start the environment:
```
docker-compose up
```

* Run artisan:
```
docker-compose exec web php artisan
```

* Run migration:
```
docker-compose exec web php artisan migration
```

* Check out the mysql database:
Browse to localhost:8180

* Stop the environment:
```
docker-compose stop
```

Enjoy!
