# What is this?

Setting up **docker** + **nginx** + **flask** + **vue** + **semantic** is hardly an easy task if
you want to setup production and development environments. This is my attempt
in the matter. Notice that, some containers are not complete (ux)
because, well, vue does not have a non interactive install.

## Getting started

```bash
# make sure you have fabric3 installed
# make sure to read each folder readme
# make sure you have docker and docker-compose installed

fab env:dev up  # docker-compose up in development mode
fab env:prd up  # docker-compose up in production mode
fab env:prd build  # docker-compose build in development mode
fab env:prd build  # docker-compose build in production mode
fab env:dev logs:name  # docker logs on container called <name>
fab env:prd logs:name  # docker logs on container called <name>
```

## What is what?

* app -> flask application container
* server -> nginx container
* styles -> semantic-ui container
* ux -> vuejs application container

## Changelog

**0.2**

* update to flask app dependencies (+flask-jsglue +flask-marshmallow +flask-migrate +flask-security +flask-sqlalchemy)

**0.1**

* initial version (docker + flask + vuejs + semantic-ui)