## Dockerfile for Alpine Linux

![Doom Image](../doom.jpeg) 

This Dockerfile creates a Docker container using Alpine Linux as the base image. Below are the steps to use this Dockerfile.

### Steps to Use the Dockerfile
1. Clone the repository and navigate into this directory.
2. Run the Docker build command:

   ```
   docker build -t your-alpine-image-name .
   ```
3. Run the Docker container using the command:

   ```
   docker run -it your-alpine-image-name
   ```

This will create a lightweight container based on Alpine Linux, ready for your applications.
