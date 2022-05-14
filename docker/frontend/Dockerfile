FROM node:16-alpine as node
WORKDIR /app
COPY . .
RUN npm install
RUN npm run build

FROM nginx:alpine

EXPOSE 80
COPY --from=node /app/build /usr/share/nginx/html