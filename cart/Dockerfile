FROM node:18.19.1-alpine3.19
EXPOSE 8080
RUN addgroup -S roboshop /opt/server/
USER roboshop
COPY package.json /opt/server/
COPY server.js /opt/server/
RUN npm install
CMD ["node","server.js"]