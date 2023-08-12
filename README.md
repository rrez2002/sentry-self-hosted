## Description
    install self hosted sentry

## Installation
```bash
# get generate secret key
$ sudo docker compose run --rm sentry-base config generate-secret-key
```
```bash
# in .env file 
SENTRY_SECRET_KEY=secret-key
```

```bash
# upgrade config
$ sudo docker compose run --rm sentry-base upgrade
```

## Running 
```bash
$ sudo docker compose up -d
```
