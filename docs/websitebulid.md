# 学习Markdown语法


## 创建个站步骤
!!! abstract "创建个人网站基本步骤"
     1.安装mkdocs,实现本地部署 [mkdocs部署基本流程](https://www.mkdocs.org/getting-started/)  
     2.创建Github仓库及安装Git, 通过Git部署本地内容至Github仓库   
     3.更改主题，可参考[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)

### 文件部署到仓库指令
``` shell
git init  
git add .  
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
![](https://cdn.jsdelivr.net/gh/WangTao19950912/images_for_website-@latest/images/%E6%8D%95%E8%8E%B7.PNG)
>如果强制推送命令

```text
git push -u origin main --force
```
### 将本地照片等资源上传到CDN
>CDN (Content Delivery Network) ，此处使用jsDelivr

!!! abstract "基本步骤"
     1.创建仓库  
     2.安装PicGo [PicGo下载链接](https://github.com/Molunerfinn/PicGo/releases)  
     3.配置PicGo [PicGo+Github配置及使用文档](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#github%E5%9B%BE%E5%BA%8A)  
     4.上传图片
### 遇到的问题
>1.本地文件更改后，直接通过git push -u origin main一直不能上传到仓库，
是因为不了解Git的机制，本地文件夹不是直接上传至github，而是通过Git上传，需要先将本地文件git执行才可以上传  
![](https://cdn.jsdelivr.net/gh/WangTao19950912/images_for_website-@latest/images/20250802121313645.png)  
2. PicGo不能上传图片，检查日志，询问deepseek解决
![](https://cdn.jsdelivr.net/gh/WangTao19950912/images_for_website-@latest/images/20250802122418037.png)

### 致谢和仓库
1. 感谢deepseek在代码之路给予的帮助
2. 感谢**笑笑的站**笔记参考[传送门](https://smilingwayne.github.io/me/Website/Step1/)
3.[GitHub Pages](https://www.github-zh.com/getting-started/github-pages)






 
