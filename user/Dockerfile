FROM node:20
WORKDIR /opt/server
ENV MONGO="true"
ENV REDIS_URL="redis://redis:6379"
ENV MONGO_URL="mongodb://mongodb:27017/users"
COPY package.json .
COPY *.js .
RUN npm install
CMD ["node","server.js"]