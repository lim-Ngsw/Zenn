---
title: Dockerコマンド覚書
type: tech
topics: [Docker]
published: true
slug: Memorandum of docker-command
---

自分が使ってて出てきたDockerコマンドを列記。
適宜追記や記事にしていったりすると思います。

2021.08.27 Zennへテスト投稿。当記事は[こちら](https://qiita.com/Lyme_sun/items/9c3ad968a704c3268c88)を一部改変したものとなります。

### Dockerhubにログイン
```
docker login
```

### <image>をHostへPullしてくる
```
docker pull <image>
```

### コンテナを生成してコンテナへ入る
```
docker run -it <image> bash
```

### コンテナから出る
```
exit
```

### Hostにあるコンテナの一覧を表示する（ステータスを把握する）
```
docker ps -a
```

### Hostにあるイメージの一覧を表示する
```
docker images
```

### exited状態のコンテナを再起動する
```
docker restart
```

### コンテナに対し指定したプログラムを実行する
```
docker exec -it <container> bash
```

### 生成したコンテナから新たにイメージを作る
```
docker commit <container> <image>
```

### dockerhubにあるリポジトリと同じ名前をつける
```
docker tag <source> <target>
```

### dockerhubへpushする
```
docker push <image>
```

### Hostにあるイメージを削除する
```
docker rmi <image>
```

ps = process status

exec = execute

rmi = remove image
