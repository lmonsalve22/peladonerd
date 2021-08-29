FROM httpd:2.4-alpine3.14

RUN apk add --no-cache openssh supervisor

RUN ssh-keygen -A

COPY supervisor.conf /etc/supervisor.conf

CMD [ "supervisord", "-c", "/etc/supervisor.conf" ] 
