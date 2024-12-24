# Dockerfile for 2048-game


This Dockerfile is used to build an image for the 2048-game. It uses the nginx:alpine base image and sets the working directory to /usr/share/nginx/html. It then updates the apk package manager, installs git, clones the 2048 game repository, moves the game files to the working directory, and removes the cloned repository. The image exposes port 80 and the CMD instruction starts the nginx server.

To build the image, navigate to the directory containing the Dockerfile and run the following command:

```
docker build -t 2048-game .
```

To run the image, use the following command:

```
docker run -p 80:80 2048-game
```

The 2048 game can then be accessed in a web browser at http://localhost:80.
