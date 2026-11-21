# git学习笔记
## git身份配置
- github用户名
git config --global user.name DummyStrophael
- githunb邮箱
git config --global user.email 2350645758@qq.com
- 查看配置
git config --list

## 基本工作流程：工作目录 > add > 暂存区 > commit > 本地仓库 > push > 远程仓库

## 常用命令
- 新建本地仓库: git init
- 查看改动动态：git status
- 将单个文件添加到暂存区：git add hello.md
- 添加文件夹改动：git add .
- 提交到本地仓库：git commit -m "提交备注"
- 查看提交日志: git log -oneline
- 关联远程仓库：git remote add origin https://github.com/DummyStrophael/git_bash_wang.git
- 查看远程地址：git remote  -v
- 推送到远程仓库：git push -u origin main(-u绑定默认分支)
- 拉取远程最新代码：git pull
- 克隆别人完整仓库到本地：git clone https://github.com/DummyStrophael/git_bash_wang.git
- 查看本地分支：git branch
- 创建分支：git branch dev
- 切换分支：git checkout dev
- 创建并立刻切换到新分支：git checkout -b feature/login
- 合并分支：先切回main，再合并dev：git switch main      git merge dev
- 撤销暂存（add之后，撤回暂存区，改动还在工作区）：git reset HEAD 文件名   git reset HEAD .
- 撤销工作区修改（会丢弃没add的改动)：git checkout -- 文件名
- 回退到某个提交版本：git reset --hard commitId
## 简单单人开发流程(工作目录D:/git_bash_wang)
```
git version
git config --global user.name DummyStrophael
git config --global user.email 2350645758@qq.com
cd d:/git_bash_wang
git init
git add hello.md
git commit hello.md
进入vim{输入i进入编辑模式，在第一行输入备注，按esc退出编辑模式，：wq退出}
git remote add origin https://github.com/DummyStrophael/git_bash_wang.git
it push -u origin main(推送已经成功)
修改后再次推送
git add .
git commit -m "输入备注"
git push`~
```
