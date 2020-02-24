FROM node:13.8.0-alpine3.11 as build
COPY . /app
WORKDIR /app
RUN npm i && npm run build

#
# PROD CONFIG
#
FROM nginx:1.17.8-alpine

COPY --from=build /app/build /usr/share/nginx/html
COPY ./support/prod/nginx.conf /etc/nginx/nginx.conf.template
COPY ./support/common/entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
CMD ["nginx", "-g", "daemon off;"]