# Reflection

This laboratory activity gave me a better understanding of how different services can work together to form one complete application. Instead of deploying only one container, I used Docker Compose to create a system with Nextcloud and MariaDB. Nextcloud served as the application that users could access through a browser, while MariaDB handled the database requirements of the application.

One thing I learned from this activity is that a docker-compose.yml file can make deployment more organized. The configuration contains the services, images, ports, and environment variables needed by the application. Once the file was prepared, I only needed to run docker compose up -d to start the whole stack. This was more convenient than manually creating and configuring every container.

I also learned that YAML files require correct indentation. A small formatting mistake can cause Docker Compose to reject the configuration. Because of this, I had to pay attention to the spaces used in the file and make sure the structure was correct.

Environment variables were another important part of the activity. Variables such as MYSQL_PASSWORD, MYSQL_DATABASE, and MYSQL_USER provided the information needed for the connection between Nextcloud and MariaDB. The MYSQL_HOST=database setting was especially important because it allowed Nextcloud to locate the database service through its Docker Compose service name.

The activity also showed me the advantage of using containers for application deployment. The web application and database were separated into their own services, but they could still communicate through Docker's network.

Overall, this mission increased my confidence in using Docker Compose and the Linux terminal. I now have a clearer idea of how Infrastructure as Code can simplify the deployment of applications with multiple components.
