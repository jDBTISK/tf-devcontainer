# Terraform Devcontainer

## Overview

vscode の [devcontainer](https://code.visualstudio.com/docs/remote/containers) を利用した terraform 開発環境

## Description

- terraform
- tfsec
- awscli
- session manager plugin

がインストールされたコンテナを作成します。

### Parameters

`.devcontainer/.env.example` を参考に `.devcontainer/.env` を作成することで、以下の変数に任意の値を設定可能です

| name        | description                         | required | default               |
| ----------- | ----------------------------------- | :------: | --------------------- |
| TF_VERSION  | terraform version                   |          | latest                |
| BASHRC_PATH | コンテナ内で利用する .bashrc のパス |          | .devcontainer/.bashrc |
| UID         | devcontainer Linux USER ID          |          | 1000                  |
| GID         | devcontainer Linux GROUP ID         |          | 1000                  |

`.devcontainer/devcontainer.json` の `name` 属性の値もプロジェクトに応じて変えてください。
