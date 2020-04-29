FROM node:10
WORKDIR /app
COPY . .
EXPOSE 5000
ENV API_URL=http://localhost:8000
RUN npm install
CMD API_URL=$API_URL npm start
