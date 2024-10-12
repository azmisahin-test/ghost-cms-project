# Ghost CMS Project

This is a simple project using Ghost CMS with Docker.

## Setup

### Local Setup with Docker Compose

1. Clone the repository.
2. Run `docker-compose up -d` to start the services.
3. Access Ghost at `http://localhost:8080`.

### Production Setup with Docker Stack

You can also deploy this project in a production-like environment using Docker Stack.

1. Clone the repository.
2. Run `docker stack deploy -c stack.yml ghost` to deploy the stack.
3. Access Ghost at the IP address of your Docker host, typically at `http://<your-ip>:8080`.

### Play with Docker Setup

You can also quickly deploy this project using Play with Docker.

1. Go to [Play with Docker](https://labs.play-with-docker.com/).
2. Click on "Start" to create a new instance.
3. In the terminal, run the following command to deploy the stack:

   ```bash
   docker stack deploy -c https://raw.githubusercontent.com/azmisahin-test/ghost-cms-project/main/stack.yml ghost
   ```

4. Access Ghost at the IP address provided in Play with Docker, typically at http://<your-ip>:8080.

### Environment Variables

MYSQL_ROOT_PASSWORD: The root password for MySQL.

MYSQL_DATABASE: The name of the database to be created for Ghost.

MYSQL_USER: The user for the Ghost database.

MYSQL_PASSWORD: The password for the Ghost database user.

### Notes

Docker Compose is ideal for local development and testing.

Docker Stack is suited for production environments and allows for distributed deployments across multiple hosts.


## Accessing Your Ghost Site
After setting up your Ghost CMS, you can access your site at the following URL:

Site URL: http://localhost:8080/

You can log in to the admin panel by appending /ghost to the URL:

Admin Panel URL: http://localhost:8080/ghost
