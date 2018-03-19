当误用了其余邮箱push或其他手残脑残操作导致github没有记录下contributions时适用

使用指南：

1、创建一个待修改的git项目的clone并进入

git clone --bare https://github.com/XXXX/XXXX.git

cd XXXX.git

2、下载change.sh脚本，并将其中的用户名用户邮箱相关的三个变量值替换为你想要的对应值

3、运行change.sh脚本，并使用git log检查是否修改为想要的

4、push改动

git push --force --tags origin 'refs/heads/*'

5、删除本地的clone
