FROM node:10
WORKDIR /usr/app
COPY . .
EXPOSE 8000
ENV FRONT_URL=http://localhost
RUN npm install
CMD FRONT_URL=$FRONT_URL npm start
