FROM nginx:alpine

COPY /default/ /red/default/
COPY /site1/ /red/site1/
COPY /site2/ /red/site2/

COPY default.conf /etc/nginx/conf.d/default.conf

EXPOSE 3001