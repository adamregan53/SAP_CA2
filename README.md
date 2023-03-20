Branch name: main

```
docker network create mysql
docker run --network mysql -e MYSQL_ROOT_PASSWORD=my-secret-password --name mysql -d mysql:latest
docker run --network mysql -p 83.212.127.135:8080:80 -e PMA_HOST=mysql -d phpmyadmin/phpmyadmin
```

