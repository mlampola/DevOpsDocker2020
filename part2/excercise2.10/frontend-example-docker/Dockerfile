FROM node:10
WORKDIR /app
COPY . .
EXPOSE 5000
ENV API_URL=http://localhost/api/
RUN npm install
CMD API_URL=$API_URL npm start
