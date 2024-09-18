# XXL-JOB

已废弃

~~自动发布项目到 docker hub, 以便让极空间 pull 到来部署 xxl-job-admin~~

~~本项目: https://github.com/alfredoo7/xxl-job~~

源项目: https://github.com/xuxueli/xxl-job

## ~~注意点~~

```yml
# CICD 需配置 
DOCKER_USERNAME = 账号
DOCKER_PASSWORD = 密码
DOCKER_TOKEN = 你的 docker AT
RELEASE_TOKEN = 你的 github AT

  # docker tag 读取该文件
version.keep
```

```yml
# 文件夹路径需设置，将 logback 日志挂载到宿主机
/data = /M.2存储12/xxl-job/data

# 环境 PARAMS 需设置，注入数据库地址 
PARAMS = --spring.datasource.url=jdbc:mysql://xxx:3306/xxl_job?useUnicode=true&characterEncoding=UTF-8&autoReconnect=true&serverTimezone=Asia/Shanghai --spring.datasource.username=root --spring.datasource.password=xxx
```