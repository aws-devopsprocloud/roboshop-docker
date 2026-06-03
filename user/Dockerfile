FROM node:20
EXPOSE 8080 
WORKDIR /opt/server
ENV MONGO="true"
ENV REDIS_URL="redis://redis:6379"
ENV MONGO_URL="mongodb://mongodb:27017/users"
ENV MONGO_URL="mongodb://mongodb:27017/catalogue"
COPY server.js /opt/server
COPY package.json /opt/server
RUN npm install 
CMD ["node", "server.js"]



