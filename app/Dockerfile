FROM alpine:latest as app

ENV DB_USER=${DB_USER} \
    DB_PASSWORD=${DB_PASSWORD} \
    DB_NAME=${DB_NAME}
    
WORKDIR /opt/express

RUN apk --update add git npm &&\
    git clone https://github.com/alexkonkin/nodejs-mysql-crud.git .

CMD ["node","./app.js"]
#CMD ["/bin/sh"]









