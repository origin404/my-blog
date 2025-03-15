>>### 1. Node.js 原生命令
>>运行脚本
>>```bash
>>    node app.js          # 直接运行 JS 文件
>>    node -e "console.log('Hello')"  # 直接执行代码片段
>>```   
>>​调试模式
>>```bash
>>    node inspect app.js  # 启动调试器（Chrome DevTools 协议）
>>    node --inspect-brk   # 在首行断点暂停，用于连接调试工具
>>```
>>​查看环境变量
>>```bash
>>    node -p "process.env.PATH"  # 打印 PATH 环境变量
>>```
>
>>### ​2. npm/npx 核心操作
>>包管理（npm）​
>>```bash
>>    npm init -y                  # 快速生成 package.json
>>    npm install express          # 安装包（写入 dependencies）
>>    npm install -D nodemon       # 安装开发依赖（devDependencies）
>>    npm uninstall lodash         # 卸载包
>>    npm update                   # 更新所有依赖
>>    npm list --depth=0           # 查看已安装的顶层依赖
>>```
>>​快速执行（npx）​
>>```bash
>>    npx create-react-app my-app  # 临时下载并执行命令（无需全局安装）
>>    npx http-server              # 快速启动本地静态服务器
>>    npx nodemon app.js           # 直接运行本地 nodemon
>>```
>
>>### 3. 实用工具命令
>>​自动重启服务器(nodemon)  
>>```bash
>>    npm install -g nodemon   # 全局安装
>>    nodemon app.js           # 修改文件后自动重启
>>```
>>​进程管理（pm2）​
>>```bash
>>    npm install -g pm2
>>    pm2 start app.js         # 启动应用
>>    pm2 list                 # 查看运行中的进程
>>    pm2 restart app          # 重启
>>    pm2 delete app           # 停止并删除
>>```
>>​代码检查（ESLint）​
>>```bash
>>    npx eslint app.js        # 检查代码规范
>>    npx eslint --init        # 生成配置文件
>>```  
