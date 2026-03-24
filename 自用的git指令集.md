#自用的git指令集

###拉取当前文件内容和推送相关

```bash
git add           #添加相关文件
git commit -u      #提交文件
git push -u origin main			#推送到Github
git pull origin main		#拉取最新代码
git diff --cached --name-only				#检查当前暂存区文件
git push -f				#强制提交
```

###移除相关文件

```bash
git reset HEAD README.md 	#移除单个文件
git reset HEAD				#移除所有暂存文件
```

###拉取远程代码

```bash
git pull
```

###查看全局配置

```bash
git config --global --list
git checkout main      #检查是否当前分支
```

###查看当前仓库的远程地址

```bash
git remote -v
```

###查看当前分支

```bash
git branch
```

###查看仓库状态

```bash
git status
git diff --cached --name-only #快速查看暂存区文件
```

###连接远程仓库

```bash
git remote add origin 你的仓库地址
git remote set-url origin https://github.com/mengbanfu/新仓库名.git
```

###查看提交记录

```bash
git log --oneline    #查看当前路径下提交记录
```

###Github上的提交流程   (举例)

```bash
echo "# mygit" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/mengbanfu/mygit.git
git push -u origin main
```

