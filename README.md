# Basic Lamp Stack Using Docker

This project is a basic example for how to use Docker to manage the various pieces of the lamp stack without installing software onto the host system.

## Installation

This project uses Docker and assumes `docker` and `docker-compose` are installed on the host operating system.

This project can be launched using.

```
$ docker-compose build
```

Followed by

```
$ docker-compose up
```

After running `docker-compose up` you can access the project in the browser at `localhost:8086/`. Anything that is put into the `src` folder will be served to the client.

## Database

The database connection is hosted at the address of 'mysql'. This is a docker network address and references the internal address.

The default database credentials are:

db address: mysql

Database: appdb

User: user

Password: pass

These values are located in the `docker-compose.yml` file and should be changed to different values when serving from a production server.
