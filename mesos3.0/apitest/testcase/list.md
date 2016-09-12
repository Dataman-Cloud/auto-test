#finushed
用户管理
登录 /v1/login     ok ok 
登出 /v1/logout    ok ok
修改密码 /v1/password ok ok ok
创建用户 /v1/accounts ok ok 
获取所有用户 /v1/accounts ok 
获取指定用户信息 /v1/accounts/:account_id ok ok
获取当前用户信息 /v1/aboutme ok
注销一个用户 /v1/account/:account_id/disable ok

主机管理
获取集群主机列表 /v1/nodes ok
获取集群监控信息 ok
获取指定主机的信息 ：/v1/nodes/:node_ip/info ok ok 
获取指定主机的容器列表 /v1/nodes/:node_ip/instances ok ok
获取指定主机的镜像列表 /v1/nodes/:node_ip/images ok ok
获取主机上指定容器的信息 /v1/nodes/:node_ip/instances/:instance_id/info  ok
删除指定主机上的指定镜像 /v1/nodes/:node_ip/images/:image_id

#need to do
获取主机上指定容器的日志 /v1/nodes/:node_ip/instances/:instance_id/logs
获取主机上指定容器的状态 /v1/nodes/:node_ip/instances/:instance_id/stats
应用管理
获取应用列表 /v1/apps
新建应用 /v1/apps
获取指定应用的信息 /v1/apps/:aid
获取指定应用的状态 /v1/apps/:aid/stats
获取指定应用的日志 /v1/apps/:aid/logs
更新指定应用 /v1/apps/:aid
重启指定应用 /v1/apps/:aid/restart
删除指定应用 /v1/apps/:aid
获取指定应用所有实例 /v1/apps/:aid/tasks
获取指定应用所有版本 /v1/apps/:aid/versions
根据应用版本id获取版本信息 /v1/apps/:aid/versions/:version
杀掉列出的任务实例并根据请求扩缩应用 /v1/tasks/delete
获取所有等待执行的任务实例 /v1/queue
版本信息
版本 /v1/version
健康检查
健康检查 /v1/health

