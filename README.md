# prometheus

此為 TSDB 測試用 docker 文件.

先決條件:

- 安裝 [Docker-desktop][docker] ( 安裝方式請參考 [Docker-Document][dokcer_doc] ).
- 安裝 [WSL2][wsl2_docs].

## 啟動方式:

將目錄放置於 wsl 路徑.
```shell
# 切換至 wsl 路徑, 預設為
cd \\wsl.localhost\Ubuntu\home\<yourname>
```

創建新資料夾並進入.
```shell
mkdir <YourFolderName>
cd <YourFolderName>
```

拉取 git.
```shell
git clone https://github.com/Zheweihu/prometheus.git
```

啟動 docker
```shell
# 切換至 docker-compose.yml 路徑
cd docker

# 啟動 docker
docker compose up -d
```

若要重新啟動或關閉 docker

```shell
# 重新啟動 docker
docker compose restart

# 關閉 docker
docker compose down -v
```

成功開啟 docker 後可進入
- [prometheus][prometheus]
- [grafana][grafana]
- [node-exporter][node-exporter]
- [cadvisor][cadvisor]

<!-- link -->
[prometheus]: http://localhost:9090
[grafana]: http://localhost:3000
[node-exporter]: http://localhost:9100
[cadvisor]: http://localhost:8080

[docker]: https://www.docker.com/products/docker-desktop/
[dokcer_doc]: https://docs.docker.com/desktop/install/windows-install/
[wsl2_docs]: https://learn.microsoft.com/en-us/windows/wsl/install