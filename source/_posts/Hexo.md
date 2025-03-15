# Hexo的搭建
> hexo博客搭建
## 一.安装Node.js和git
### node.js是一款主要用于服务器端开发的工具.  
可以做到让Javascript直接运行在服务器上，用于构建高性能的网络应用  
主要用途为构建Web服务器.实时应用.API服务.代理服务器,服务器渲染等  
安装于D:\New Folder\node.js  
### Git 是分布式版本控制工具.  
常用于代码管理、团队开发、版本发布、文档追踪  
​记录变更,保存代码/文件的所有修改历史，可回退到任意版本  
​高效协作,多人同时修改同一项目，自动合并或提示冲突  
分支管理,独立开发新功能（分支），测试通过后合并到主代码  
>数据安全,本地和远程仓库双重备份，代码永不丢失  
基础命令:commit(提交).push/pull(同步).merge合并).clone(下载仓库)  
安装于C:\Program Files\Git  
注:git的作用中大部分可被github desktop替代(基于Git的远程代码托管平台)  
而Git作为本地版本控制工具，核心是管理文件变更  
>检验  
>```bash  
>    node -v
>    npm -v
>    git --version  
>```  

### 外：安装cnpm(安装Hexo)  
```bash  
    npm install -g cnpm --registry=https://registry.npmmirror.com  
```  
cnpm,是由淘宝团队维护的Node.js包管理工具.  
它是 npm/yarn 的替代品.默认使用国内的 pmmirror.com​(原淘宝 NPM 镜像)来加速依赖载.  
适合在中国大陆等网络访问境外npm官方源较慢的景  
安装后  
```bash  
   added 1 package in 20s
   59 packages are looking for funding
   run `npm fund` for detail
```
意为成功安装了 1 个包  
当前项目依赖的 59 个包（开源项目）正在寻求资支持可使用npm fund查看相关详情  
关闭资助提示(配置 npm 全局忽略资助提示)
>```bash
>  npm config set fund false --global
>```
# 二.安装Hexo
Hexo是一个基于Node.js的静态博客生成器.可将 Markdown 文件快速渲染成静态网页.支持主题和插件，适合搭建轻量.高效的个人博客或文档站点.  
在全局安装 Hexo 命令行工具
```bash
  npm install hexo-cli -g
```  
>检验  
>```bash
>  hexo -v
>``` 
# 三.Github配置
建立Github仓库,在GitHub/GitHub desktop中新建一个库并起名my-blog，拉取或推送上去，保证两端同步 
在my-blog中重复连接国内服务器.全局安装hexo.