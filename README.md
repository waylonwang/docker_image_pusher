# Docker Images Pusher

使用Github Action将国外的Docker镜像转存到私有仓库，供国内服务器使用，免费易用<br>
支持DockerHub, gcr.io, k8s.io, quay.io, ghcr.io等任意仓库

原作者：**[技术爬爬虾](https://github.com/tech-shrimp/me)**<br>
具体使用参见原作者[说明](https://github.com/tech-shrimp/docker_image_pusher/blob/main/README.md)

## 本Fork个性化修订:
* 不使用阿里云私有库，改用转存到自托管的私有库
* 从Github上Swarm stacks repo的docker-compose文件中提取#image-ref键值中的镜像路径进行转存
* 使用Registry V2的API判断目标私有库如已有镜像版本则不重复转存