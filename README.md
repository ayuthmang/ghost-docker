## How to use ?

1. Create a `.env` file in root project folder and put

```
MYSQL_ROOT_PASSWORD=<SUPER_SECRET_PASS>
```

2. Edit ghost url in file `docker-compose.yml` in `url` to `http://<YOUR_URL>`

3. Edit nginx config file in `nginx/conf/ghost.conf` on section `server_name` to your domain name for example my domain name is `ghost.local`

```
server {
    listen 0.0.0.0:80;
    server_name ghost.local;
    access_log /var/log/nginx/ghost.local;
    .
    .
}
```

4. Run the environment

```bash
$ docker-compose up -d
```

5. Access to your url for example my url is `http://ghost.local`
