FROM alpine:latest

RUN apk add --no-cache \
    neovim \
    curl \
    wget \
    git \
    python3 \
    py3-pip \
    nodejs \
    npm \
    gcc clang \
    ripgrep \
    fd \
    tree-sitter \
    unzip gzip \
    bash

RUN npm install -g neovim
RUN apk add --no-cache py3-pynvim

COPY nvim/init.lua /root/.config/nvim/init.lua

CMD ["nvim"]
