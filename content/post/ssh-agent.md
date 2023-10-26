+++
title = 'ssh-agentの使い方'
date = 2023-10-26T12:32:45+09:00
draft = false
tags = ["ssh"]
+++

Githubにpushする際、ssh-agentの使い方で躓いたのでメモがわりに。

<!--more-->
## ssh-agentの起動
```
$ eval `ssh-agent`
```
## ssh-agentの停止
```
$ ssh-agent -k
```

## ssh-addの使い方
```
ssh-add [秘密鍵のパス]
```
秘密鍵をssh-agentに登録。
```
ssh-add -L
```
登録されている鍵の公開鍵一覧を表示。
```
ssh-add -d [秘密鍵のパス]
```
登録されている鍵を削除。