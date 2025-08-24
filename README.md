# dockerでマイクラ構築

## ホワイトリスト
### サーバの設定変更
- server.propertiesを変更
```
- white-list=false
+ white-list=true
```

### ユーザ追加
- https://api.mojang.com/users/profiles/minecraft/ユーザ名でuuidを確認
- whitelist.jsonにユーザ追加
```json
[
  {
    "uuid": "hogehoge-piyo-piyo-hoge-hogepiyopiyo",
    "name": "user1"
  },
  {
    "uuid": "piyopiyo-hoge-hoge-piyo-piyohogehoge",
    "name": "user2"
  }
]
```
