FROM nginx:alpine

RUN apk add --no-cache gettext

COPY index.html /usr/share/nginx/html/index.html.template

CMD ["/bin/sh", "-c", "envsubst '$STUDENT_NAME' < /usr/share/nginx/html/index.html.template > /usr/share/nginx/html/index.html && exec nginx -g 'daemon off;'"]

