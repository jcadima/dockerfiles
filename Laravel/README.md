### Make sure to create the following directory and file:
```
/docker-compose/nginx/laravel.conf
```

Note container-name needs to match the one declared at docker-compose.yml
```
fastcgi_pass laravel-admin:9000;
```

#### List of container names
```
docker ps --format "{{.Names}}"
```

#### Access App Container
```
docker exec -it your-app-container bash
```

#### Access Mysql Container
```
docker exec -it your-db-container mysql -u your-db-user -p
```
