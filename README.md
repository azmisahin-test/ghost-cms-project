# Ghost CMS Project

This is a simple project using Ghost CMS with Docker.

## Setup

### Local Setup

1. Clone the repository.
2. Run `docker-compose up -d` to start the services.
3. Access Ghost at `http://localhost:2368`.

### Play with Docker Setup

You can also quickly deploy this project using Play with Docker.

1. Go to [Play with Docker](https://labs.play-with-docker.com/).
2. Click on "Start" to create a new instance.
3. In the terminal, run the following command to deploy the stack:

   ```bash
   docker stack deploy -c https://raw.githubusercontent.com/azmisahin-test/ghost-cms-project/main/stack.yml ghost
   ```

4. Access Ghost at the IP address provided in Play with Docker, typically http://<your-ip>:2368.

### Environment Variables

MYSQL_ROOT_PASSWORD: The root password for MySQL.

MYSQL_DATABASE: The name of the database to be created for Ghost.

MYSQL_USER: The user for Ghost database.

MYSQL_PASSWORD: The password for Ghost database user
