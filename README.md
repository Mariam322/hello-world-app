# hello-world-app

Service Harice (`hello-world-app`), genere automatiquement par le Maestro.

- Type : nest
- Port : 2002
- Image : systeodigital/hello-world-app

Le CI/CD est automatique : a chaque push, Jenkins build l'image,
la pousse, puis la deploie via `docker compose` sur le serveur.
Le `Jenkinsfile` et le `docker-compose.yml` sont deja prets.

## En local
```bash
docker build -t systeodigital/hello-world-app:dev .
docker run --rm -p 2002:2002 systeodigital/hello-world-app:dev
```
