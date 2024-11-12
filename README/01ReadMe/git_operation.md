# ！！！一定要切换到自己的分支，不要在master主分支中直接编辑

1.查看当前在哪个分支
```
git branch
```

2.切换到自己的分支中
```
git checkout cpy_branch
git checkout zs_branch
git checkout lyc_branch
git checkout wxj_branch
```

3.将master主分支的内容同步到自己当下的分支，保证自己当下的分支的内容是最新的
```
(1) git checkout wxj_branch    切换到要同步的子分支
(2) git merge master           将主分支的内容同步到子分支上
(3) git status                 在子分支查看当前的代码状态
```

4.在自己的分支中进行编码。。。  
5.查看当前的代码状态（发现有未提交的）
```
git status
```
6.将代码添加到本地仓库
```
git add .
```
7.为本次提交添加注释，解释你做了什么
```
git commit -m "修复了xxx.c中的问题..."
```
8.将本地仓库中的代码上传到git服务器，上传后可以在github的自己的分支中看到已经更新了，但是master主分支中仍是更新前的样子
```
git push origin HEAD
```
9.合并当前分支内容到master主分支
```
git checkout master
git merge wxj_branch
```
