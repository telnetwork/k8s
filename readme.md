```shell
mkdir basic
cd basic
git init
git config --global user.name "xxx"
git config --global user.email "xxx@qq.com"
git config --global --list
git status
# 已修改/创建  工作区
echo 'this is a test file' > test_file.txt
# 已暂存   提交到暂存区
git add test_file.txt  # git add .
git status
# 已提交   提交到Git仓库，远程仓库
git commit -m "create test_file.txt"
git status
```
