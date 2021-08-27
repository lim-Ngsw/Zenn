自分が使ってて出てきたDockerコマンドを列記。
適宜追記や記事にしていったりすると思います。

2021.08.27 Zennへテスト投稿。当記事は[こちら](https://qiita.com/Lyme_sun/items/9c3ad968a704c3268c88)と
同一のものになります。

```
docker login // dockerhubにログイン
docker pull <image> // <image>をHostへpullしてくる
docker run -it <image> bash // コンテナを生成してコンテナへ入る
exit //　コンテナから出る
docker ps -a // Hostにあるコンテナの一覧を表示する（ステータスを把握する）
docker images // Hostにあるイメージの一覧を表示する
docker restart // exited状態のコンテナを再起動する
docker exec -it <container> bash // コンテナに対し指定したプログラムを実行する
docker commit <container> <image> // 生成したコンテナから新たにイメージを作る
docker tag <source> <target> // dockerhubにあるリポジトリと同じ名前をつける
docker push <image> // dockerhubへpushする
docker rmi <image> // Hostにあるイメージを削除する
```

ps = process status

exec = execute

rmi = remove image
