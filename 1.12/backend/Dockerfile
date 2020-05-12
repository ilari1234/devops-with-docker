FROM ubuntu

WORKDIR /backendapp

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash 
RUN apt-get install -y nodejs

COPY . .

RUN node -v && npm -v
RUN npm install

ENV FRONT_URL=http://localhost:5000

CMD npm start