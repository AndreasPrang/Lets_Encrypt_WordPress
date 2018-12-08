# Docker-App: WordPress with SSL-Offloader and Let's Encrypt
WordPress with Let's Encrypt


## Dependencies:
- Install Docker-App (announced at DockerCon 18 Europe): https://github.com/docker/app
- Let`s encrypt needs a publicly accessible domain to issue certificates.

## Start Docker App
```
#create folder to store certificates, database and wordpress uploads
mkdir </persistant/data/path>

git clone https://github.com/AndreasPrang/Lets_Encrypt_WordPress.git
cd Lets_Encrypt_WordPress
docker-app render --set data_path=</persistant/data/path> \
                  --set domain=<my.domain.ltd> \
                  --set email=<mail@domain.ltd> \
                  --set letsencrypt_test=<true|false>  \
                  | docker-compose -f - up -d
```
