# Home Assitant学习


## 部署
!!! abstract "部署在docker的几种方法"

     1.部署在windows docker中 
     2.部署在linux docker中 
   

### 部署到windows docker中的几个要点

> 不要忘记端口号，可能造成无法访问8123端口界面
```shell
# 1. 停止当前容器
docker stop Home_assitant

# 2. 删除当前容器（不用担心，你的配置在映射的卷里，不会丢失）
docker rm Home_assitant

# 3. 重新运行容器，这次务必加上 -p 8123:8123
docker run -d `
  --name home-assistant `  # 建议使用更标准的命名，例如用减号代替下划线
  -v C:/Users/1111/docker/homeassistant/config:/config `  # 请确保这个目录存在且路径正确
  -p 8123:8123 `          # <--- 这是最关键的一步，添加端口映射
  --restart unless-stopped `
  homeassistant/home-assistant:latest
```
> 常用指令
```shell
docker run ... 或 docker-compose up -d：启动。
docker stop 和 docker start：停止和启动。
docker logs -f：排查问题。
docker exec -it ... /bin/bash：进入容器内部。
docker restart home-assistant 重启

```
```shell
docker ps：查看状态。
```
![](https://raw.githubusercontent.com/WangTao19950912/images_for_website-/main/images20250826212448519.png)

>HA界面访问地址
http://192.168.31.147:8123/ ，*192.168.31.147*替换为主机IP

>安装HACS至HA
![](https://raw.githubusercontent.com/WangTao19950912/images_for_website-/main/images20250826221302902.png)
[HACS学习链接](https://hacs.xyz/docs/use/configuration/basic/#to-set-up-the-hacs-integration)


### 致谢和仓库
1. 感谢deepseek在代码之路给予的帮助  
2. 







 
