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
git status
# 已暂存   提交到暂存区
git add test_file.txt  # git add .
git status
# 已提交   提交到Git仓库，远程仓库
git commit -m "create test_file.txt"
git status


# 创建GitHub仓库后，添加GitHub仓库到本地
git remote add k8s git@github.com:telnetwork/k8s.git  # add后面的 k8s 名称可以自定义
git remote



# SSH key
ssh-keygen -t rsa -b 2048 -C "xxx@qq.com"   # .pub 是公钥

# 1. 复制公钥的里的内容
# 2. 打开GitHub页面 ----->> 点击右上角头像 ----->> 点击Settings ----->> 点击左边的 SSH and GPG keys ----->> 点击右上角的 New SSH key 
#    ----->> Title：可选 | Key type：默认 | Key：粘贴刚才的公钥内容 ----->> 最后点击Add SSH key 

ssh -T git@github.com  # yes

git push -u k8s main  # k8s 就是上面定义的远程仓库名称


git log
```
