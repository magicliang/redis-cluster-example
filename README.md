# redis-cluster-example
Redis cluster的实例网络

## 灵感

inspired by redis-sentinel-example.

## notes

- 每个哨兵需要单独的配置文件，以防每个进程往里面写东西相互覆盖
- 每个的 cluster 的 node 也使用单独的配置文件。
- cluster 模式默认不能开 slaveof，所以不要在配置文件或者命令行中出现 slaveof（在命令行中使用 slaveof 还会和配置文件相冲突）。

## 启动方案

```bash
# TODO：silent化，制作 sop 启动方式，attach 方式和日志切入方式
docker-compose up
```
