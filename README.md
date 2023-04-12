# MeuSite (guiaguirres.dev.br)

Para subir o site:

``` shell
docker-compose up -d
```

Para instalar previamente o certificado SSL:

``` shell
docker-compose run --rm  certbot certonly --webroot --webroot-path /var/www/certbot/ --dry-run -d guiaguirres.dev.br
```

Para fixar a instalação do certificado:

``` shell
docker-compose run --rm  certbot certonly --webroot --webroot-path /var/www/certbot/ -d guiaguirres.dev.br
```

Para renovar o certificado:

``` shell
docker-compose run --rm  certbot renew
```
