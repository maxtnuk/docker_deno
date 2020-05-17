FROM rust:slim

USER root
# install python
RUN apt-get update
RUN apt-get install -y python3
RUN update-alternatives --install /usr/bin/python python /usr/bin/python3 1 \
    && python --version
RUN cargo install deno

ENV DENO_INSTALL="/root/.deno"

