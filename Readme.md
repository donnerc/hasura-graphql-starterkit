# Hasura starter kit

## Configuration

### Starting the NGINX proxy and setting up HTTPS

```bash
cd nginx-letsencrypt
docker-compose up -d
```

From now on, all docker container started with special environment variables `LETSENCRYPT_HOST`, `LETSENCRYPT_EMAIL` and `VIRTUAL_HOST` will be accessible under HTTPS behind NGINX with a Let's Encrypt signed certificate.

### Starting Hasura

1.  Copy the file `.env.template` to `.env`
2.  Configure the variables in `.env` file
3.  run `source .env` to load the env vars
4.  run `docker-compose up -d`
5.  enjoy

