# phpimage

## イメージの作成
- docker build . -t myphpimage

## コンテナの起動
- docker run -dit --name myphp -p 8080:80 myphpimage

## ブラウザで確認
- http://localhost:8080

## 後始末
- docker stop myphp
- docker rm myphp

## イメージをファイル化する
- docker save -o saved.tar myphpimage

## イメージファイルから読み込む
- docker load -i saved.tar

## Docker Hubのアカウントを作成する
- https://hub.docker.com/

## イメージをDocker HubにPushする
- docker tag myphpimage 自分のdocker id/myphpimage
- docker login
- docker push 自分のdocker id/myphpimage
