## Docker Compose for WordPress

![WordPress Online Image](https://www.vectorlogo.zone/logos/wordpress/wordpress-icon.svg)
![Docker Compose Image](https://www.vectorlogo.zone/logos/docker/docker-icon.svg)

This Docker Compose file sets up a WordPress environment with a MySQL database. Below are the steps to use this Docker Compose file.

### Steps to Use the Docker Compose File
1. Use the following curl command to download the Docker Compose file directly into this directory:

   ```
   curl -o docker-compose.yml https://raw.githubusercontent.com/yourusername/yourrepository/main/Wordpress/docker-compose.yml
   ```
2. Run the Docker Compose command:

   ```
   docker-compose up -d
   ```
3. Access your WordPress site by navigating to `http://localhost` in your web browser.

**Note:** You can change the ports in the `docker-compose.yml` file, but changing the port of MySQL is not recommended.

This will create a WordPress environment with a MySQL database, ready for your applications.
