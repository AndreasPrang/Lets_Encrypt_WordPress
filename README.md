# Docker-App: WordPress with SSL-Offloader and Let's Encrypt
WordPress with Let's Encrypt


## Dependencies:
- Install Docker-App (announced at DockerCon 18 Europe): https://github.com/docker/app
- Let`s encrypt needs a publicly accessible domain.

## Start Docker App
```
git clone https://github.com/AndreasPrang/Lets_Encrypt_WordPress.git
cd Lets_Encrypt_WordPress
docker-app render --set domain=<my.domain.ltd> --set email=<mail@domain.ltd> --set letsencrypt_test=<true|false>  | docker-compose -f - up -d
```
