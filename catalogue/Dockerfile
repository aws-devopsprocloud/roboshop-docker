FROM node:20
EXPOSE 8080 
WORKDIR /opt/server
ENV MONGO=true
COPY server.js /opt/server
COPY package.json /opt/server
RUN npm install 
CMD ["node", "server.js"]



