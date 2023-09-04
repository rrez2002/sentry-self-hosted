## Description
**install self hosted sentry**

# Installation
**get generated secret key**
~~~bash
$ sudo docker compose run --rm sentry-base config generate-secret-key
~~~

**change to .env file**

`SENTRY_SECRET_KEY`=secret-key

**upgrade config**
~~~bash
$ sudo docker compose run --rm sentry-base upgrade
~~~

**Running**
~~~bash
$ sudo docker compose up -d
~~~

**open to browser:  [Sentry Login](http://0.0.0.0:9000/)**


#