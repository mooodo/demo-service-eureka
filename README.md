# demo-service-eureka
这是一个项目用于演示微服务的注册中心eureka。
该项目演示了如下内容：
### 多套环境配置
在bootstrap.yml文件中编写了多套环境配置：
```
dev:       本地开发环境配置
docker:    单节点docker容器部署配置
cluster:   在kubernetes云端集群配置
primary:   docker集群配置的第一个节点
secondary: docker集群配置的第二个节点
tertiary:  docker集群配置的第三个节点
```
### Kubernetes容器化部署
在根目录下编写k8s容器化部署的yaml文件：
```
demo-service-eureka.yaml          单节点部署
demo-service-eureka-cluster.yaml  注册中心集群
```
注意：在进行集群部署时，更多的配置信息在配置中心config中，详解demo-service-config