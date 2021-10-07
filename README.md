# k8s
#思路：先部署代码，然后部署nats/redis/mongdb
/*
操作1：部署代码
步骤1：编写compose文件部署代码
https://github.com/moleculerjs/moleculer-examples/blob/master/blog/docker/micro/docker-compose.yml
1)配置容器运行环境
2)从仓库拉取镜像
步骤2：使用docker-compose让镜像部署到k8s
-------------------------------------------
操作2：部署nats镜像
1)直接拉取远端仓库nats镜像编排文件
docker search nats
docker pull nats:latest
2)k8s编排文件对应nats-dockerCompose.yml
-------------------------------------------
操作3：部署redis镜像
1)直接拉取远端仓库redis镜像编排文件
docker search redis
docker pull redis:latest
2)k8s编排文件对应redis-dockerCompose.yml

-------------------------------------------
操作4：部署mongdb镜像
1)直接拉取远端仓库mogdb镜像编排文件
docker search mongo
docker pull mongo:latest
2)k8s编排文件对应mogdb-dockerCompose.yml
*/
