## Web Application Tier

The web application tier is responsible for handling requests from users and displaying the application's interface. In this deployment, Nextcloud serves as the web application. Users can access Nextcloud through a web browser, while the application handles the requests and communicates with the database.

## Database Tier

The database tier is responsible for storing information required by the application. MariaDB is used in this deployment to store Nextcloud data such as user information, settings, and other application-related records.

## Why Separate the Tiers?

Separating the application and database into different containers makes the system more organized. Each container has its own responsibility, which makes it easier to manage, update, and troubleshoot the services. The two containers can still communicate through the Docker network while remaining separate services.
