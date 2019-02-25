## How to use ?

1. Create a .env file in root project folder. with

```
MYSQL_ROOT_PASSWORD=<SUPER_SECRET_PASS>
```

2. Edit nginx config file in `nginx/conf/ghost.conf` on section `server_name` to your domain name for example my domain name is ghost.local

```
server {
    listen 0.0.0.0:80;
    server_name ghost.local;
    access_log /var/log/nginx/ghost.local;
    .
    .
}
```

3. Run the environment

```bash
$ docker-compose up -d
```

4. Access to your url.