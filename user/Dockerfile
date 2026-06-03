FROM node:20
EXPOSE 8080 
WORKDIR /opt/server
ENV MONGO="true"
ENV MONGO_URL="mongodb://mongodb:27017/catalogue"
ENV REDIS_URL="redis://redis:6379"
COPY server.js /opt/server
COPY package.json /opt/server
RUN npm install 
CMD ["node", "server.js"]


# FROM node:20
# # this creates /app and move there
# WORKDIR /app
# ENV MONGO="true" \
#     MONGO_URL="mongodb://mongodb:27017/catalogue" \
#     REDIS_URL="redis://redis:6379"
# EXPOSE 8080
# COPY package.json .
# COPY *.js .
# RUN npm install
# CMD ["node", "server.js"]
