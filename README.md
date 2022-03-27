# docker使用

## 镜像
#### docker源设置
- 编辑/etc/docker/daemon.json
```
{
  "registry-mirrors" : [
    "http://ovfftd6p.mirror.aliyuncs.com",
    "http://registry.docker-cn.com",
    "http://docker.mirrors.ustc.edu.cn",
    "http://hub-mirror.c.163.com"
  ],
  "insecure-registries" : [
    "registry.docker-cn.com",
    "docker.mirrors.ustc.edu.cn"
  ],
  "debug" : true,
  "experimental" : true
}
```
- 然后重启docker
#### 镜像搜索
```
docker image search
```
#### 镜像拉取
```
docker image pull 镜像名
```
#### 镜像列出
```
docker image ls
```
#### 镜像删除
```
docker image rm 镜像名
```
#### 将某个容器上传为镜像
```
docker commit 镜像名 容器名
```

## 容器
#### 容器创建
```
docker container create 参数
```
