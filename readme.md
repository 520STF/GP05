# readme文档
- 项目说明文档
- 一般都与项目放一起

# git操作

## 初始化版本库
- git init
- 初始化成功后，当前目录后面有(master)
- 初始化成功后当前目录下有个隐藏文件.git（不要管，不要操作这个文件）

## 工作区
- 持有实际文件
- 我们平时增删改查的文件都是工作区的内容

## 提交到暂存区
- 可以理解为我们看不到的一个地方
- 是存在于用户电脑中的
- 本地仓库的一个主要组成部分

## 本地仓库
- 也可以理解为我们看不到的一个地方
- 也是存在于用户电脑中的
- 用于存储项目代码及版本相关记录等信息


## 提交到暂存区
- git add 文件名
- 将工作区的一些变动(增删改)提交到暂存区
- git add . 将所有变动提交到暂存区

## 查看工作区和暂存区的状态
- git status
- 查看工作区和暂存区的状态(增删改)

## 提交到本地仓库
- git commit -m '提交注释'
- 将代码从暂存区提交到本地仓库
- git status 查看状态：提示工作区是干净的，没有任何东西需要提交

## 本地操作关键步骤
1. git init
(仅仅是第一次需要写，看本地文件是否有隐藏的 .git 文件)
2. git add .
3. git commit -m "注释"

## 查看日志
-- git log  查看完整日志
-- git reflog   查看简单日志

## 版本回退
- git reset --hard HEAD^
回退到上一个版本
- git reset --hard 版本号
回退到制定版本
- 注意吧当前代码先提交到本地仓库
- 工作区的代码自动变成恢复的指定版本的代码

## 退出编辑区
- : wq
