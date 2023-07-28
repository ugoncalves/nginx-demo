FROM nginxinc/nginx-unprivileged:latest
#FROM nginx

COPY nginx.conf /etc/nginx/template_nginx.conf
COPY script.sh /etc/nginx/.

EXPOSE 8080

ENTRYPOINT [ "/bin/bash", "/etc/nginx/script.sh", "/etc/nginx/template_nginx.conf", "/etc/nginx/nginx.conf"]
