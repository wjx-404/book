### 什么是 git？
+ 是一个源代码管理工具
+ 在一个项目中，凡是由开发人员编写的就算源代码
+ 源代码为什么需要管理？ 用意是什么？
  + 人为管理和维护比较麻烦
  + 可以让源代码可以被追溯，主要记录每次变更了什么，谁主导的这次变更
+ GIT是Linux之父当年为了维护Linux的源代码编写的一个工具
+ 在git之前都用什么？
  + SVN vss tfs...

### git基本命令

+ 初始化一个仓库
```shell
cd  项目根目录
$ git init  初始化一个本地仓库
```

> 就是在我们本地文件夹中 添加一个.git文件夹用于记录所有的项目变更信息

+ 查看本地仓储的变更状态
```shell
$ git status
$ git status -s
```

+ 添加本地需要托管的文件
```shell
$ git add <file>
$ git add --all  &&  git add .
```

+ 类似于node_modules这种性质的文件夹不应该被托管

+ 添加一个本地git的忽略清单文件
> 在代码库文件夹的根目录添加一个.gitignore文件，该文件用于说明忽略文件有哪些

+ 提交被托管的代码变化到本地仓库
```shell
$ git commit -m '...'
```


+ 设置名字和email
```shell
$git config --global user.email "you@example.com"
$git config --global user.name "Your Name"
```

+ 提交被托管的代码变化的本地仓库
```shell
$ git commit -m "..."
```

+ 回到指定版本
```shell
$ git reset --hard
```

+ 查看提交日志
```shell
$ git log
```

+ 对比差异
```shell
$git diff
```

### github是什么？
> GitHub说白了只是一个网站
> 同性交友社区 都是程序员
> https://github.com/
> 提出概念：社交化编程平台，同时他也是git的服务提供商
+ GitHub和git的关系：他是git的服务提供商，提供了免费的仓库，--前提：开源