FROM httpd:2-alpine3.19

RUN apk add --no-cache openssh supervisor

RUN ssh-keygen -A

COPY supervisor.conf /etc/supervisor.conf

CMD [ "supervisord", "-c", "/etc/supervisor.conf" ] 
