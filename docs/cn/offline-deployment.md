# 离线部署

通过自托管 draw.io 来替代 `embed.diagrams.net`，从而离线部署 Next AI Draw.io。

**注意：** `NEXT_PUBLIC_DRAWIO_BASE_URL` 是一个**构建时**变量。修改它需要重新构建 Docker 镜像。



## 配置与重要警告

**`NEXT_PUBLIC_DRAWIO_BASE_URL` 必须是用户浏览器可访问的地址。**

| 场景 | URL 值 |
|----------|-----------|
| 本地主机 (Localhost) | `http://localhost:8080` |
| 远程/服务器 | `http://YOUR_SERVER_IP:8080` |

**切勿使用** Docker 内部别名（如 `http://drawio:8080`），因为浏览器无法解析它们。
