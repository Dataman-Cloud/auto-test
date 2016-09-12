#[HOW TO USE](../pyresttest/advanced_guide.md)





##已完成
- [用户管理](#用户管理)
  - [登录 /v1/login](#登录)
  - [登出 /v1/logout](#登出)
  - [修改密码 /v1/password](#修改密码)
  - [创建用户 /v1/accounts](#创建用户)
  - [获取所有用户 /v1/accounts](#获取所有用户)
  - [获取指定用户信息 /v1/accounts/:account_id](#获取指定用户信息)
  - [获取当前用户信息 /v1/aboutme](#获取当前用户信息)
  - [注销一个用户 /v1/account/:account_id/disable](#注销一个用户)
- [主机管理](#主机管理)
  - [获取集群主机列表 /v1/nodes](#获取集群主机列表)
  - [获取集群监控信息 /v1/metrics/snapshot](#获取集群监控信息)
  - [获取指定主机的信息 /v1/nodes/:node_ip/info](#获取指定主机的信息)
  - [获取指定主机的容器列表 /v1/nodes/:node_ip/instances](#获取指定主机的容器列表)
  - [获取指定主机的镜像列表 /v1/nodes/:node_ip/images](#获取指定主机的镜像列表)
  - [获取主机上指定容器的信息 /v1/nodes/:node_ip/instances/:instance_id/info](#获取主机上指定容器的信息)

- [应用管理](#应用管理)
  - [获取应用列表 /v1/apps](#获取应用列表)
  - [新建应用 /v1/apps](#新建应用)
  - [获取指定应用的信息 /v1/apps/:aid](#获取指定应用的信息)
  - [更新指定应用 /v1/apps/:aid](#更新指定应用)
  - [重启指定应用 /v1/apps/:aid/restart](#重启指定应用)
  - [删除指定应用 /v1/apps/:aid](#删除指定应用)
  - [获取指定应用所有实例 /v1/apps/:aid/tasks](#获取指定应用所有实例)
  - [获取指定应用所有版本 /v1/apps/:aid/versions](#获取指定应用所有版本)
  - [根据应用版本id获取版本信息 /v1/apps/:aid/versions/:version](#根据应用版本id获取版本信息)
  - [杀掉列出的任务实例并根据请求扩缩应用 /v1/tasks/delete](#杀掉列出的任务实例并根据请求扩缩应用)
  - [获取所有等待执行的任务实例 /v1/queue](#获取所有等待执行的任务实例)
- [版本信息](#版本信息)
  - [版本 /v1/version](#版本)
- [健康检查](#健康检查)
  - [健康检查 /v1/health](#健康检查)

##未完成 测试框架目前满足不了
  - [删除指定主机上的指定镜像    /v1/nodes/:node_ip/images/:image_id](#删除指定主机上的指定镜像)
  - [获取主机上指定容器的日志 /v1/nodes/:node_ip/instances/:instance_id/logs](#获取主机上指定容器的日志)
  - [获取主机上指定容器的状态 /v1/nodes/:node_ip/instances/:instance_id/stats](#获取主机上指定容器的状态)
  - [获取指定应用的状态 /v1/apps/:aid/stats](#获取指定应用的状态)
  - [获取指定应用的日志 /v1/apps/:aid/logs](#获取指定应用的日志)