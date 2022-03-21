# Terraform Devcontainer

## Overview

vscode の [devcontainer](https://code.visualstudio.com/docs/remote/containers) を利用した terraform 開発環境

## Description

- terraform
- tfsec
- tflint
- awscli

がインストールされたコンテナを作成します。

### Parameters

`.devcontainer/.env.example` を参考に `.devcontainer/.env` を作成することで、以下の変数に任意の値を設定可能です

| name        | description                          | required | default               |
| ----------- | ------------------------------------ | :------: | --------------------- |
| ARCH        | CPU アーキテクチャ (arm64 or x86_64) |          | x86_64                |
| TF_VERSION  | terraform version                    |          | latest                |
| BASHRC_PATH | コンテナ内で利用する .bashrc のパス  |          | .devcontainer/.bashrc |
| UID         | devcontainer Linux USER ID           |          | 1000                  |
| GID         | devcontainer Linux GROUP ID          |          | 1000                  |
