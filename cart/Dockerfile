FROM node:20
EXPOSE 8080 
WORKDIR /opt/server
ENV REDIS_HOST="redis"
ENV CATALOGUE_HOST="catalogue"
ENV CATALOGUE_PORT="8080"
ENV HERO="Prem"
COPY server.js /opt/server
COPY package.json /opt/server
RUN npm install 
CMD ["node", "server.js"]