FROM deno:init

WORKDIR /install

COPY deno.tar /install/deno.tar

RUN tar xvf deno.tar
RUN cd deno/cli && cargo install --path .

RUN deno --version

ENV DENO_INSTALL="/root/.deno"

