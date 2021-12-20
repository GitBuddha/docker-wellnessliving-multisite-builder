# WP/React Multisite Builder

## Precondition

- `cp env-example .env`
- `mkdir dbfile react4multisite wp-multisite`

### Git WordPress

- `git clone git@github.com:wellnessliving/wp-multisite.git ./wp-multisite`
- `git checkout development`
- `mv ./docker/wordpress/config/wp-config.php ./wp-multisite`

### Git React

- `git clone git@github.com:wellnessliving/react4multisite.git ./react4multisite`
- `git checkout development`
- `mv /docker/wordpress/config/build_local.sh ./react4multisite/dev_build`
- `cd react4multisite/dev_build`
- `bash build_local.sh`

## Run Docker Image

- `docker-compose up -d`

## Stop Docker Image

- `docker-compose down`

## PhpMyAdmin

- `http://localhost:8080/`
