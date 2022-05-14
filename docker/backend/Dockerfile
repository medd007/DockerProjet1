FROM node:16-alpine as node-builder
WORKDIR /app
COPY --chown=node:node . .
RUN npm install --legacy-peer-deps

CMD ["npm", "start", "--trace-warnings"]