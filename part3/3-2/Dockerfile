FROM ubuntu:16.04

RUN apt-get update && apt-get install -y \
    python3.5 wget ffmpeg python3-pip && \ 
    pip3 install pycrypto && \ 
    pip3 install yle-dl && \ 
    apt-get purge -y python3-pip && \ 
    rm -rf /var/lib/apt/lists/*

WORKDIR /app

ENTRYPOINT ["/usr/local/bin/yle-dl"]
