FROM nginx:alpine

COPY /default/ /green/default/
COPY /site1/ /green/site1/
COPY /site2/ /green/site2/

COPY default.conf /etc/nginx/conf.d/default.conf

EXPOSE 3000