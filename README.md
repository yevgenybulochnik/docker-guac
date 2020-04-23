# Apache Guacamole Docker Compose
This repo contains a docker-compose setup to create guacamole, guacd and postgres containers. The database image uses docker multistage build to generate the correct guacd tables. The guacd server also uses multistage builds to install powerline fonts and ttf-ancient-fonts.

# Env Vars
```
POSTGRES_USER
POSTGRES_PASSWORD
POSTGRES_DATABASE
```
