## Dockerfile for Website from Github Repository

<span><img src="https://www.vectorlogo.zone/logos/w3_html5/w3_html5-icon.svg" alt="HTML Logo" width="50" height="50" /></span>
<span><img src="https://www.vectorlogo.zone/logos/w3_css/w3_css-official.svg" alt="CSS Logo" width="50" height="50" /></span>
<span><img src="https://www.vectorlogo.zone/logos/javascript/javascript-icon.svg" alt="JavaScript Logo" width="50" height="50" /></span>
<span><img src="https://www.vectorlogo.zone/logos/github/github-tile.svg" alt="JavaScript Logo" width="50" height="50" /></span>

This Dockerfile creates a Docker container using Alpine Linux as the base image for Website. Below are the steps to use this Dockerfile.
You can find my website at: [My Website](https://dhruvmistry2000.github.io/dhruvmistry/)


### Steps to Use the Dockerfile
1. Clone the repository from GitHub: [My GitHub Repository](https://github.com/dhruvmistry2000/mydocker) and navigate into this directory.
2. Run the Docker build command:

   ```
   docker build -t your-image-name .
   ```
3. Run the Docker container using the command:

   ```
   docker run -it -p 8080:80 your-image-name
   ```

This will create a lightweight container based on Alpine Linux, ready for your applications. You can also find this image on my Docker Hub page: [Mywebsite Image](https://hub.docker.com/repository/docker/dhruvmistry200/mywebsite/general).

**Caution:** Make sure to change the repository link in the Dockerfile to your own repository link before building the Docker image.
