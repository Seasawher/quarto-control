FROM mcr.microsoft.com/devcontainers/base:jammy

# ユーザの追加
USER vscode
WORKDIR /home/vscode
ENV HOME=/home/vscode

# quarto のインストール
ARG QUARTO_VERSION=1.6.32
RUN wget https://github.com/quarto-dev/quarto-cli/releases/download/v${QUARTO_VERSION}/quarto-${QUARTO_VERSION}-linux-amd64.deb && \
  sudo apt install ./quarto-${QUARTO_VERSION}-linux-amd64.deb

