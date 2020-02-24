FROM nginx:1.17.8-alpine

COPY ./support/dev/proxy/nginx.conf /etc/nginx/nginx.conf.template
COPY ./support/common/entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

EXPOSE 3000
ENTRYPOINT ["/entrypoint.sh"]
CMD ["nginx", "-g", "daemon off;"]