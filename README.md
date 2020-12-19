# Django React graphql Template

Full featured django react template so that you can get to your work started immediately

### Development

-   Just do `docker-compose up -d`
-   your app will be there at localhost:8000

```
Note: db_interface/ does not work right now , for now to access pgadmin go to localhost:8080/
```

### Deployment

The app is full ready to be deployed on heroku.

#### Steps

-   Install heroku cli
-   `heroku create`
-   `heroku config:set SECRET_KEY=yoursecret DJANGO_SETTINGS_MODULE=backend.settings.production`
-   Add postgresql addon
    -   `heroku addons:create heroku-postgresql:hobby-dev`
-   `heroku stack:set container`
-   `git push heroku master`

Deployed!!
