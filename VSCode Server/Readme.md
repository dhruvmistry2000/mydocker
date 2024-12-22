## VSCode Server with Docker Compose

<span><img src="https://code.visualstudio.com/assets/images/code-stable.png" alt="VSCode Logo" width="50" height="50" /></span>
<span><img src="https://www.vectorlogo.zone/logos/docker/docker-icon.svg" alt="Docker Logo" width="50" height="50" /></span>

This setup creates a VSCode Server instance using Docker Compose. The server provides a browser-based VSCode environment that you can access from anywhere.

### Steps to Use Docker Compose
1. Create a directory for your project.

2. Download the docker-compose.yml file using curl:

   ```
   curl -o docker-compose.yml https://raw.githubusercontent.com/dhruvmistry2000/mydocker/main/VSCode%20Server/docker-compose.yml
   ```

3. Configure your environment:
   - Open docker-compose.yml and modify the PASSWORD environment variable to set your desired password
   - Uncomment and modify the volumes section to map your desired workspace directory:
     ```yaml
     volumes:
       - /path/to/your/workspace:/home/coder/project
     ```

4. Start the VSCode server using:

   ```
   docker-compose up -d
   ```

5. Access VSCode in your browser at:

   ```
   http://localhost:8081
   ```

The default password is "your_password", but you should change this to something secure by modifying the PASSWORD environment variable in docker-compose.yml before starting the container.

**Note:** The volumes mapping allows you to persist your workspace and access local files. Make sure to set the correct path to your workspace directory when uncommenting this section.
