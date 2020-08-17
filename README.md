# Image CMS Grav

Ce repo est un clone du dépôt officiel réalisé pour une instance docker déployé sur un NAS Synology.

Pour l'installer sur un NAS synology (testé sur un RS820), Vous devez préalablement avoir installé le service docker à partir du centre de paquets.

### Création du répertoire de persistance  
Par defaut, une fois lancé, l'image **docker** lance une installation propre de GRAV. Mais vous ne pourrez pas accéder directement aux dossiers hébergeant la structure **GRAV**.  
Pour cela il vous est possible de créer dans votre NAS, un répertoire sur lequel le volume de perssitance docker va se brancher. Vous pouvez même y charger la structure complête de votre futur site GRAV.  
>> ATTENTION : Vous devez attribué les droits en écriture à l'ensemble des dossiers et fichiers pour que l'instance Docker puisse communiquer avec votre dossier, pour que vos modification puisse être prise en compte. 


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

