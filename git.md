# git
版本管理工具

主要有两种
集中式版本控制系统  SVN         分布式版本控制系统 git
git init 初始化git
git add 添加文件到暂存区
git commit -m "备注说明"   将暂存区里的内容一次性提交到版本库中
master 分支

git status  显示项目状态
git log --pretty=oneline  版本日志

git reset --hard hash值  回退指定版本
git reset --hard HEAD^   回退前1个版本
git log  查看的版本日志
git status  查看项目状态
git diff  比较文件在工作区和暂存区的对比


reset  版本回退
撤销修改：
在还没有将文件add时，又修改了内容并且不想要，快速撤销回到该文件最新一次add时的状态
文件已经add了，先回退上commit 提交1个版本，然后再从暂存区里取出内容覆盖工作区里的文件

分支： 版本时间线，master分支默认为主分支
作用：
## 查看分支
git branch

## 创造分支
git branch abb

## 切换分支
git checkout

## 合并分支：
git merge dev

## 删除分支
 git branch -d abb

合并冲突： 合并分支时，如果两个分支在同名文件的同一个位置有两套完全不同的修改，git 是没法智能决定保留谁丢弃谁
HEAD相当于一个指针，指向当前正在开发的分支master，master指向最新的提交
