# はじめに

本ソースコードは、
https://zenn.dev/faycute/articles/9024115c4241b8
を参考にしております。

## 動作確認コマンドメモ

### コマンドから（何度も確認したい場合）

```bash
python -c "import app; app.lambda_handler(None, None)"
```

### コンテナを起動して確認

```bash
docker-compose up --build
curl -d '{}' http://localhost:9000/2015-03-31/functions/function/invocations
```
