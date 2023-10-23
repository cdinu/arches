FROM mcr.microsoft.com/devcontainers/python:1-3.11-bullseye
ENV PYTHONUNBUFFERED 1
RUN apt update
RUN apt install -y mc neovim postgresql-client curl
RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
RUN export NVM_DIR="/usr/local/share/nvm"
RUN [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" && nvm install 16 && npm install -g yarn

