## Services Block

The services block contains the containers that make up the application. This deployment has two services: database and app. The database service runs MariaDB, while the app service runs Nextcloud.

## Database Service

The database service uses the mariadb:10.6 image. Its environment variables define the root password, database password, database name, and database user. These settings allow MariaDB to create the database that Nextcloud will use.

## Application Service

The application service uses the nextcloud image. It provides the web interface of the private cloud system. Port 8080 on the host is connected to port 80 inside the Nextcloud container.

## How Nextcloud Finds MariaDB

Nextcloud uses the following environment variable:

MYSQL_HOST=database

The value database refers to the name of the MariaDB service in the Compose file. Docker Compose provides an internal network where the containers can communicate using their service names.

## Environment Variables

Environment variables are used to provide configuration values to the containers. In this deployment, they are used for database credentials, the database name, and the database host. This keeps the configuration separate from the application image.

## Docker Run vs Docker Compose

docker run is normally used to create and start a container through an individual command. Docker Compose is designed for applications that require multiple related containers. Instead of entering many commands, the services and their settings can be defined in one YAML file and deployed together using docker compose up -d.
