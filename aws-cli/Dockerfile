# AWS CLI2 を利用するDockerfile
FROM python:3.9

# 前提パッケージのインストール
RUN apt-get update && apt-get install -y less vim curl unzip sudo

# aws cli v2 のインストール
# https://docs.aws.amazon.com/ja_jp/cli/latest/userguide/install-cliv2-linux.html
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-aarch64.zip" -o "awscliv2.zip"
RUN unzip awscliv2.zip
RUN sudo ./aws/install

# ENV PATH $PATH:/usr/local/bin/
# RUN complete -C '/usr/local/bin/aws_completer' aws

WORKDIR /workdir