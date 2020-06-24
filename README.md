# Image CMS Grav

Ce repo est un clone du dépôt officiel réalisé pour une instance docker déployé sur un NAS Synology.
Elle est en cours de test à ce jour.

### Notes depuis le repo officiel de https://getgrav - Image pour le CMS GRAV

This currently is pretty minimal and uses:

* apache-2.4.38
* GD library
* Unzip library
* php7.3
* php7.3-opcache
* php7.3-acpu
* php7.3-yaml
* cron
* vim editor

#### Building the image from Dockerfile

```
docker build -t grav:latest .
```

#### Running Grav Image with Latest Grav + Admin:

```
docker run -p 8000:80 grav:latest
```

Point browser to `http://localhost:8000` and create user account...

#### Running Grav Image with Latest Grav + Admin with a named volume (can be used in production)

```
docker run -d -p 8000:80 --restart always -v grav_data:/var/www/html grav:latest
```
