# A Fast Wordpress with a web-based filebrowser

For local development ( or production use )

## Deployment

To deploy wordpress + filebrowser using single Docker Compose filebrowser just simply run :

```sh
docker-compose up -d
```

## Services

- MySQL ( localhost : 12305 )
- Wordpress ( <http://localhost:9070/> )
- Filebrowser ( <http://localhost:9071/> )

## Notes

Wordpress & MySQL services will use a mounted docker volume ( :delegated : this is for fast run in local environments)

Filebrowser will use ./filebrowser folder for it's db file and json config file, also mounted to your wordpress_data volume to browse and edit wordpress files & folders via web

<b>You can change all host ports for development purposes or production</b>
