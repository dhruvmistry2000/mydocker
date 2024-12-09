# Start Generation Here
FROM nginx:alpine

# Set the working directory
WORKDIR /usr/share/nginx/html

# Clone the GitHub repository into a temporary directory and move files
RUN apk add --no-cache git && \
    git clone https://github.com/dhruvmistry2000/dhruvmistry /tmp/repo && \
    cp -r /tmp/repo/* . && \
    rm -rf /tmp/repo

# Expose port 80
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]
# End Generation Here
