# 学习Markdown语法


## 设计logo图片，放置在images文件夹中


!!! abstract "使用chatgpt设计logo"
     图片的含义，TTP，TaoTao Partner 
     这是第二段  
     这是*斜体*  
     这是**粗体**  

    《大浴女》
## 文件部署到仓库指令
``` shell
git init
```
```shell
git add .
```
```text
git commit -m "init repo"
```
> 这里的 `init repo` 可以更换成任意描述，用来概括你此次提交代码的行为。
```shell
git branch -M main
```
```shell
git remote add origin https://github.com/WangTao19950912/WangTao19950912.github.io

```
>不是每次必须要建立连接
 ```shell
    git push -u origin main
 ```
强制推送命令
```text
git push -u origin main --force
```
## 将本地照片等资源上传到CDN
>CDN (Content Delivery Network) ，此处使用jsDelivr

!!! abstract "jsDelivr"
 
