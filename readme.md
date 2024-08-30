```shell
mkdir basic
cd basic
git init
git config --global user.name "xxx"
git config --global user.email "xxx@qq.com"
git config --global --list
git status
echo 'this is a test file' > test_file.txt
git add test_file.txt  # git add .
git status
git commit -m "create test_file.txt"
git status
```
