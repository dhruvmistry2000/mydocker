## Dockerfile for MyWebsite

<span><img src="https://upload.wikimedia.org/wikipedia/commons/6/61/HTML5_logo_and_wordmark.svg" alt="HTML Logo" width="50" height="50" /></span>
<span><img src="https://upload.wikimedia.org/wikipedia/commons/9/99/CSS3_logo_and_wordmark.svg" alt="CSS Logo" width="50" height="50" /></span>
<span><img src="https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png" alt="JavaScript Logo" width="50" height="50" /></span>

This Dockerfile creates a Docker container using Alpine Linux as the base image for MyWebsite. Below are the steps to use this Dockerfile.
You can find my website at: [My Website](dhruvmistry2000.github.io/dhruvmistry/)


### Steps to Use the Dockerfile
1. Clone the repository from GitHub: [My GitHub Repository](https://github.com/dhruvmistry2000/dhruvmistry) and navigate into this directory.
2. Run the Docker build command:

   ```
   docker build -t your-alpine-image-name .
   ```
3. Run the Docker container using the command:

   ```
   docker run -it your-alpine-image-name
   ```

This will create a lightweight container based on Alpine Linux, ready for your applications. You can also find this image on my Docker Hub page: [Mywebsite Image](https://hub.docker.com/repository/docker/dhruvmistry200/mywebsite/general).
