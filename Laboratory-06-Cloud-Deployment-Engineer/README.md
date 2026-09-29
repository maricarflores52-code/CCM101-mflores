## Mission Overview

This laboratory focused on deploying a private cloud storage application using multiple Docker containers. Nextcloud was used as the web application, while MariaDB was used as the database. Docker Compose was used to configure and manage both services.

## Objectives

- Learn the basic structure of a multi-tier application.
- Create a Docker Compose configuration file.
- Deploy Nextcloud and MariaDB as separate containers.
- Understand communication between containers.
- Access the deployed application through a web browser.
- Practice Infrastructure as Code concepts.

## Commands Executed

mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker compose up -d
docker compose ps
docker compose down

## Skills Learned

This activity improved my understanding of Docker Compose, YAML configuration, container networking, environment variables, and multi-tier application deployment. I also practiced using Linux commands to create directories, edit configuration files, start containers, check their status, and shut down the deployment.
