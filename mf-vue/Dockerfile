# Building APP
FROM node:20.12-alpine AS build

WORKDIR /app

COPY . . 

RUN npm ci --silent
RUN npm run build

# Starting NGINX
FROM nginx:1.25.4

COPY ./nginx.conf /etc/nginx/nginx.conf
COPY --from=build /app/dist /usr/share/nginx/html
