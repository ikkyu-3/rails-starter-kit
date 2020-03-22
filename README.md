# rails-starter-kit

## 前提

- Docker DesktopがインストールされているPC

## 使い方

```sh
./tools/docker-up.sh # 起動
./tools/docker-exec.sh my-app # my-appにアクセス

# my-app container
$ rails new .
$ rails s -b '0.0.0.0'
```

`http://localhost:3000`にアクセス
