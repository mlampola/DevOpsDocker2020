FROM node:10.16.0-alpine as build-stage
WORKDIR /app
COPY . .
RUN npm install && \
    npm run build

FROM node:10.16.0-alpine
WORKDIR /app
COPY --from=build-stage /app/dist/ /app/dist
EXPOSE 5000
ENV API_URL=http://localhost/api/
RUN npm install -g serve && \
    adduser -D app && \
    chown -hR app /app
USER app
CMD API_URL=$API_URL serve -s -l 5000 dist

