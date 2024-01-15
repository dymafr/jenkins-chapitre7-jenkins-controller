# Pour créer le certificat initial

```
sudo docker run -it --rm \
  -p 80:80 \
  -v "./data/certbot/conf:/etc/letsencrypt" \
  -v "./data/certbot/www:/var/www/certbot" \
  certbot/certbot certonly \
  --standalone \
  --agree-tos \
  --email VORE_EMAIL \
  -d VOTRE_DOMAINE
```
# jenkins-chapitre7-jenkins-controller
