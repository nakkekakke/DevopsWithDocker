FROM ubuntu:16.04
EXPOSE 8000
WORKDIR /mydir
COPY . /mydir

RUN apt-get update && apt-get install -y curl bash
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install
CMD ["npm", "start"]
