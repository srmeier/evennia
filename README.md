# ProjCon

Custom Evennia Docker image.

```
docker build . -t registry.digitalocean.com/projcon/evennia
docker login -u <token> -p <token> registry.digitalocean.com
docker push registry.digitalocean.com/projcon/evennia
docker run -it --user root -v <local_dir>:/usr/src/game registry.digitalocean.com/projcon/evennia
apk update && apk add postgresql-dev
pip install psycopg2-binary
evennia --init projcon
evennia migrate
evennia createsuperuser
```
