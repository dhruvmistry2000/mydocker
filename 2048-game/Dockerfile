FROM nginx:alpine

WORKDIR /usr/share/nginx/html
RUN apk update && apk add git && \
    git clone https://github.com/gabrielecirulli/2048.git && \
    mv 2048/* . && \
    rm -rf 2048

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]