FROM node:20.20-alpine3.22
EXPOSE 80/tcp
ENV DB_HOST=mysql
RUN addgroup -S expense && adduser -S expense -G expense
RUN mkdir /opt/server
RUN chown expense:expense -R /opt/server/
WORKDIR /opt/server/
COPY package.json .
COPY *.js  /opt/server/
RUN npm install
CMD ["node","index.js"]