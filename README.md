# ProjCon

Custom Evennia Docker image.

```
docker build https://github.com/srmeier/evennia.git#projcon-dev -t registry.digitalocean.com/projcon/evennia
docker login -u <token> -p <token> registry.digitalocean.com
docker push registry.digitalocean.com/projcon/evennia:dev
docker run -it --user root -v <local_dir>:/usr/src/game registry.digitalocean.com/projcon/evennia:dev
evennia --init projcon
evennia migrate
evennia createsuperuser
```
