# Docker-App: WordPress with SSL-Offloader and Let's Encrypt
WordPress with Let's Encrypt


## Dependencies:
Install Docker-App (announced at DockerCon 18 Europe): https://github.com/docker/app

## Start Docker App
```
docker-app render --set domain=<my.domain.ltd> --set email=<mail@domain.ltd> --set letsencrypt_test=<true|false>  | docker-compose -f - up -d
```
