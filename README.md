# registry
registry k8s 部署 方案

+ 启动服务
```shell
helm install your-registry ./registry -n your-namespace
```
+ 修改daemon.json
```shell
  "insecure-registries": [
    "192.168.32.89:30050"
  ]
  
systemctl restart docker
```

+ 登陆镜像仓库
```shell
docker login 192.168.32.89:30050
```


