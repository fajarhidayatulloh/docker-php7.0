## Docker-PHP7.0

A quick and easy way to setup your PHP application using Docker and docker-compose. This will setup a developement environment with PHP7.0-fpm, Mysql and Nginx.

## Usage
~~~
git clone git@github.com:fajarhidayatulloh/docker-php7.0.git
cd docker-php7.0
docker-compose up
~~~

### Structure

~~~
├── apps
│   └── public
├── database
├── docker-compose.yml
├── fpm
│   ├── Dockerfile
│   └── supervisord.conf
├── nginx
│   ├── Dockerfile
│   └── default.conf
~~~

- `apps` is the directory for project files. Our Nginx config is pointing to `apps/public`, which can be changed in `nginx/default.conf`
- `database` is where Mysql will store the database files.

