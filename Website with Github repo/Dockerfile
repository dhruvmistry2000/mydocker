FROM nginx:alpine

WORKDIR /usr/share/nginx/html

RUN apk add --no-cache git && \
    git clone --depth 1 https://github.com/your_username/your_repository_name /tmp/repo && \
    cp -r /tmp/repo/* . && \
    rm -rf /tmp/repo

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]