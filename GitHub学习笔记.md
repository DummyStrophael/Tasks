##  一.基础概念

1.	仓库（Repository ）：存放项目代码、版本记录的地方，分本地仓库、远程仓库（GitHub上）
2.	工作区：电脑里项目文件夹，你直接编辑文件的地方
3.	暂存区（Stage 和 Index）：临时存放准备提交的改动
4.	本地仓库：.git 隐藏文件夹，保存所有历史版本快照
5.	提交（commit）：保存一个版本，必须写简短说明，每个 commit 有唯一哈希id
6.	分支（branch）：独立开发线，互不干扰，默认主分支 main（旧项目常是 master）
7.	远程（remote）：指向GitHub仓库的地址，默认别名 origin
## 二.SSH 免密登录
1.	生成密钥：ssh-keygen -t ed25519 -C
2.	一路回车，生成公钥 id_ed25519.pub
3.	复制公钥内容，去 GitHub Settings  SSH and GPG keys 新增SSH Key
4.	测试连接：ssh -T git@github.com，提示成功即生效
之后远程地址改用 SSH 链接，不再需要密码
## 三.GitHub 平台核心功能
1.	README.md：项目首页说明，使用 Markdown，项目门面，写清楚：项目介绍、环境、安装、使用方法
2.	Issues：任务、bug反馈、需求讨论，可打标签、分配负责人
3.	Fork：复刻别人仓库到自己账号（开源贡献第一步）
4.	Pull Request（PR）：提交改动给原仓库作者，经过代码评审（Code Review）后合并 开源贡献流程：Fork → clone到本地 → 新建分支修改 → push自己fork仓库 → 提PR
5.	GitHub Pages：把静态网页、Markdown笔记免费部署成网站
6.	GitHub Actions：CI/CD自动化，自动测试、打包、部署、检查代码
## 四.Commit 提交注释规范
   1.feat: 新增功能
   2.fix: 修复bug
   3.docs: 修改文档、注释、README
   4.style: 格式调整，无代码逻辑变化
   5.refactor: 代码重构，不新增功能、不修bug
   6.test: 增加/修改测试代码
   7.chore: 构建、依赖、工程配置改动
## 五.踩过的坑
   1.编辑完没提交
   2.写错了格式

## 六.GitHub主页编辑
使用在线工具[profile readme generator](https://profile-readme-generator.com/en)编辑，参考了克劳德 https://github.com/elementalsouls/Claude-BugHunter skillevaluate https://github.com/NVIDIA/SkillEvaluator
本人主页地址：https://github.com/DummyStrophael
