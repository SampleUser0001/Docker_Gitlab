# Docker Gitlab

## コマンド
```
docker run --detach \
  --publish 443:443 --publish 80:80 \
  --name gitlab \
  --restart always \
  --volume /home/ittimfn/Docker_gitlab/gitlab/config:/etc/gitlab \
  --volume /home/ittimfn/Docker_gitlab/gitlab/logs:/var/log/gitlab \
  --volume /home/ittimfn/Docker_gitlab/gitlab/data:/var/opt/gitlab \
  gitlab/gitlab-ce:9.3.11-ce.0
```


## 参考
https://qiita.com/masakura/items/e29f1dd4794bcaf066ce