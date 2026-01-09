# Syetem Network Proxy (Docker)

使用 Docker 运行网络服务

运行的前提条件是 有符合要求的正确的 `config.yaml` 文件

## 运行

1. 拷贝 `config.yaml` 文件: `cp config.copy.yaml config.yaml`

2. 配置好 `config.yaml` 正确的设置

3. 拉取linux镜像到本地: `docker pull alpine:3.18`, 如果网络不通畅, 拉取网络顺畅的镜像后重命名

4. 创建并运行: `docker compose up -d --build`, 这个是最开始需要, 后续只需要运行即可 `docker compose up -d`

## 配置

1. 登录管理看板: `http://<anyip>:9090/ui`，例如 `http://127.0.0.1:9090/ui`

2. 输入 `http://<anyip>:9090/` 作为用户，密码在 `config.yaml`有配置

3. 管理看板

## 其他

`docker-compose.yaml` 配置了端口映射, 有需要的自行调整