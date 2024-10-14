# はじめに

# 事前準備

## ネットワーク作成

```
[実行コマンド]
docker network create --subnet=172.10.10.0/24 --gateway=172.10.10.1 ecosystem

```

## volume作成
```
[実行コマンド]
docker volume create grafana-data
```