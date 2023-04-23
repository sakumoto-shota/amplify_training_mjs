# amplify_training_mjs


## ゴール
- Amplify から DynamoDBにCRUDとして APIを呼び出しCRUDアプリとして使用できるところまで

## lambdaを使用したCRUD API

- DynamoDBを使用し、lambdaから作成、更新、削除を実行する
- API Gatewayを開始、POSTMANなどでリクエストができること
- Amplify studio から APIにリクエストをし結果を描画させることができること

## DynamoDBは共通して利用するため下記をテーブル名とする

- `http-crud-training-****` の ****をそれぞれ名称を決める。

## API 一覧

```
## ****の部分はDynamoDBで作成した名前を選択する
GET /****/items/{id} ##id単位で取得
GET /****/items ##一括取得
PUT /****/items ##idを指定してupdate
DELETE /****/items/{id}
```

## 構成

![AWS図表](./images/arch.png) 

