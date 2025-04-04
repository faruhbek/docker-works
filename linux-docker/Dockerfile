# 1. Use an official Ubuntu image as the base
FROM ubuntu:22.04

# 3. Update package list and install basic tools
RUN apt-get update && \
    apt-get install -y \
    curl \
    git \
    vim \
    python3 \
    python3-pip && \
    apt-get clean
    
    
WORKDIR /app

COPY . /app

CMD [ "bash" ]

