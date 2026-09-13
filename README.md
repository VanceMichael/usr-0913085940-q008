# 翼装穿靶轨迹成绩存证接口

这是一个面向赛事运营的纯后端服务工程，提供健康检查入口、配置边界和领域模块目录。业务数据应通过 HTTP 接口进入，持久化和事件处理代码按目录职责组织。

## 运行

```bash
docker build -t sports-service .
docker run --rm -p 8080:8080 sports-service
```

服务启动后可请求 `GET /health`。配置从环境变量读取，示例配置只包含非敏感的本地值。

## 目录

- `src` 或 `cmd`：HTTP 入口与领域服务
- `tests`：后端行为测试
- `Dockerfile`：构建和运行镜像
