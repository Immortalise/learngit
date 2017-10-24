git add 文件名

把文件添加到仓库中

git commit     
 把文件提交到仓库  
后面要加 -m “”双引号内是注释

git status   
掌握当前仓库的状态

git diff  文件名
查看修改内容

"尝试一下廖雪峰教程的git方法"
"第一步 添加本文件 (文件名为 "git.md ")  成功"

mkdir 文件名
cd 文件名
pwd （显示路径）

git init（一定要init）
???
"成功使用 git status"
"第一次尝试git diff失败"
“开始第二次尝试 失败”

“使用了git log”
git log 查看修改内容 时间等
可以加上   --pretty=oneline 


“使用了git reset"
git reset --hard HEAD^(一个^代表返回到上一个版本 2个则返回上上2个版本 以此类推)
git rest --hard 版本名（不需要写全） 回到“未来”的版本

git  reflog                 --查看自己的所有行为

第一步是用git add把文件添加进去，实际上就是把文件修改添加到暂存区；
第二步是用git commit提交更改，实际上就是把暂存区的所有内容提交到当前分支。

git  checkout --文件名
这个方法可以删除你在工作区的操作
但是添加到了暂存区之后
必须再添加一行命令
git reset HEAD 文件名

确实要从版本库中删除该文件，那就用命令git rm  文件名删掉，并且git commit -m “”
git checkout其实是用版本库里的版本替换工作区的版本，无论工作区是修改还是删除，都可以“一键还原”。





















