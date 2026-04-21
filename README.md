# How_to_use_github
关于github的一些操作命令

基础环境为 ubuntu20.04

# 配置SSH密钥
git clone自己的私有仓库时需要提前配置ssh密钥，公有仓库不需要
```shell
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
#三次Enter回车
```
将生成的公钥添加到 GitHub 账户中：
- 复制公钥内容（通常位于~/.ssh/id_rsa.pub文件中）。
- 登录 GitHub，访问 [SSH and GPG keys 设置页面](https://github.com/settings/ssh/new)。
- 粘贴公钥并保存
配置基本信息
```shell
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```
# 使用 SSH URL 克隆仓库：
```shell
git clone git@github.com:lanhuazhiyue/air_shark.git
```
# 切换分支
```shell
git checkout <branch>
```
# 提交新的修改到远程仓库
```shell
git add .
git commit -m "first commit"
git branch
git push origin <branch>
```
