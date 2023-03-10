FROM ubuntu:latest

# update & install curl
RUN apt update && apt install -y curl

# download and install go (required for hugo)
RUN curl -OL https://golang.org/dl/go1.20.2.linux-amd64.tar.gz && \
    tar -C /usr/local -xvf go1.20.2.linux-amd64.tar.gz

# export go to the environment variables
ENV PATH="${PATH}:/usr/local/go/bin"

# install hugo
RUN apt install -y hugo

# Hugo dev server port
EXPOSE 1313

