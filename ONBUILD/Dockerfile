FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
# This onbuild instruction runs only,when any user uses your images
ONBUILD COPY index.html /usr/share/nginx/index.html
CMD ["nginx", "-g", "daemon off;"]