这是一个学习ELK文档

> 在单台服务器上使用docker-compose进行部署一整套ELK
> 使用 movies 数据进行测试

```
mkder /data
cd /data
把初始数据放到/data 目录下
docker-compose ud -d

docker exec -it elasticsearch bash  # 进入es容器
cd bin
./elasticsearch-setup-passwords interactive # 设置认证密码。（为好多个账户设置密码。我这里统一都是abcd1234）
```

> 做完这些  单机版的elk就搭建完成了，测试数据已经默认导入到es，登录kibana就可以查看了
