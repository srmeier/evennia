# ProjCon

Custom Evennia Docker image.

```
docker build . -t registry.digitalocean.com/projcon/evennia
docker login -u <token> -p <token> registry.digitalocean.com
docker push registry.digitalocean.com/projcon/evennia
```
