# build environment
FROM node:12.9.0-alpine
WORKDIR /app
COPY package.json /app/package.json
COPY src /app/src
RUN npm install
RUN npm run build
EXPOSE 3000
CMD [ "node", "src/index.js" ]