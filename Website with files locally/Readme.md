## Dockerfile for Website with files locally

<span><img src="https://www.vectorlogo.zone/logos/w3_html5/w3_html5-icon.svg" alt="HTML Logo" width="50" height="50" /></span>
<span><img src="https://www.vectorlogo.zone/logos/w3_css/w3_css-official.svg" alt="CSS Logo" width="50" height="50" /></span>
<span><img src="https://www.vectorlogo.zone/logos/javascript/javascript-icon.svg" alt="JavaScript Logo" width="50" height="50" /></span>

This Dockerfile creates a Docker container using Alpine Linux as the base image for MyWebsite. Below are the steps to use this Dockerfile.
You can find my website at: [My Website](https://dhruvmistry2000.github.io/dhruvmistry/)


### Steps to Use the Dockerfile
1. Create a directory for your files and place the Dockerfile inside that directory.
2. Use the following curl command to download the Dockerfile directly into this directory:

   ```
   curl -o Dockerfile https://raw.githubusercontent.com/dhruvmistry2000/mydocker/refs/heads/main/Website%20with%20files%20locally/Dockerfile
   ```
3. Run the Docker build command from within this directory:

   ```
   docker build -t your-image-name .
   ```
4. Run the Docker container using the command:

   ```
   docker run -it -p 8080:80 your-image-name
   ```

This will create a lightweight container based on Alpine Linux, ready for your applications. You can also find this image on my Docker Hub page: [Mywebsite Image](https://hub.docker.com/repository/docker/dhruvmistry200/mywebsite/general).

**Caution:** This Dockerfile only works with vanilla HTML, CSS, and JavaScript. Ensure that your project does not include any frameworks or libraries that may not be compatible with this setup.

