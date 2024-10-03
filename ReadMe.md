# はじめに
はじめに


# 事前準備

## ネットワーク作成
ネットワークについては、サブネットを値を知っておいた方が良いので、別で定義する
```
[実行コマンド]
docker network create --subnet=172.10.10.0/24 --gateway=172.10.10.1 ecosystem

[確認コマンド]
docker network list
```

## volume 作成
```
[実行コマンド]
docker volume create grafana-data
```

## hostsファイル登録
まず、仮想サーバのIPアドレスを確認する
```
[実行コマンド]
ip a

[結果]
xxx.xxx.xxx
```
```
`val-ecosystem.com`
```

# デプロイ

```
docker compose -f docker-compose.yaml up -d
```

# 確認

コンテナのIPアドレス