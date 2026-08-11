FROM almalinux:9
RUN dnf install nginx -y
RUN mkdir /tmp/sudheer
WORKDIR /tmp/sudheer/
CMD ["nginx", "-g", "daemon off;"]