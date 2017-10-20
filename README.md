# swarm-compose-v3.3-example

## 这个是我在swarm生产环节下部署的一些基础服务，先来简单介绍下：

    cadvisor:
    google开源的容器监控插件，主要关注的是每个container的运行状态
    haproxy：
    这个目录里我使用dockercloud-haproxy这个docker官方的镜像。这个我是用来做内部7层负载均衡用的，可以选用，当然也可以选用外部的负载均衡。
    docker ingress 的网络模式配合云商提供负载均衡也完全能过解决问题
    jenkins：
    简单的jenkins例子
    ldap：
    这个是vue+django的例子。
    node_exporter:
    prometheus的插件，关注容器宿主机层面的指标
    portainer：
    重点推荐的docker环境下的web-ui。最近一些release也支持了swarm的操作。强烈推荐
    prometheus：
    prometheus监控，这里面我用了一些 docker config 的东西。
