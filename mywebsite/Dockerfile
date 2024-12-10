FROM nginx:alpine

WORKDIR /usr/share/nginx/html

RUN apk add --no-cache git && \
    git clone https://github.com/dhruvmistry2000/dhruvmistry /tmp/repo && \
    cp -r /tmp/repo/* . && \
    rm -rf /tmp/repo

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
