FROM ubuntu:16.04
EXPOSE 5000
WORKDIR /mydir
COPY . /mydir

RUN apt-get update && apt-get install -y curl bash
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install
ENV API_URL="http://localhost:8000"
CMD ["npm", "start"]
