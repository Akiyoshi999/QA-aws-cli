# 概要

このリポジトリを使用することで、DockerのAWS CLIの環境を簡単に用意することができる。
このリポジトリを作成した理由は、ローカル環境を汚さずにAWS CLIを利用したいため作成した。
AWSの試験や、CLIで確認したい場合にこの環境を使用する。

## docker コマンド

```
docker-compose up
dcoker-compose exec aws-cli-container /bin/bash
```

## AWS CLI 便利コマンド

- 認証情報確認

```
aws sts get-caller-identity
```

- AssumeRole の確認

```
aws sts assume-role --role-arn <role-arn> --role-session-name <session-name>
```

- 認証情報の設定

```
export AWS_ACCESS_KEY_ID=
export AWS_SECRET_ACCESS_KEY=
export AWS_SESSION_TOKEN=
```
