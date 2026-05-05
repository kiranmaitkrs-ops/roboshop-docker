FROM node:20
WORKDIR /app
COPY *.js .
COPY *.json .
RUN npm install
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue" \
    REDIS_URL="redis://redis:6379"
CMD ["node", "server.js"]