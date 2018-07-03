# 笔记
## 基本命令(同linux)
cd 目录移动  
mv 移动文件  
mkdir  创建目录  
cp 复制文件  
pwd 显示路径  
rm 删除文件  
ctrl+l 清屏  
ctrl+c 命令行终结  
\ 换行  
vim vim编辑模式
## 设置git参数  
### 显示当前的git配置  
git config --list  
### 设置提交仓库时的用户信息  
git config --global user.name "wjy030"  
git config --global user.email "castiel0416@hotmail.com"  
git log  
## git常用命令
git init 新建git仓库  
git clone [url] 克隆远程仓库  
git add [file1] [file2] 添加文件到暂存区  
git add . 添加所有文件到暂存区  
git rm [file1] [file2] 删除文件，并将这次删除提交到暂存区  
git mv [file-origin] [file-renamed] 改名文件，并将这次改名提交到暂存区  
git commit-m [message] 提交暂存区  
git commit -a -m [message] 直接提交工作区  
git status 显示变更信息  
git log  显示分支的历史版本  
git log --oneline  简洁版  
git show [version] 显示指定版本的提交信息  
git remote add origin https:/github.com/wjy030/hello 关连到远程仓库  
git push [remote] [branch]  推送到远程仓库分支  
git pull [remote] [branch]  从远程仓库分支拉取  
git clone [remote] 克隆远程仓库到本地  
## 一些注意点
### .gitignore  
	每行忽略一个或一类文件，可以使用globbing通配符  
### 换行符  
warning: LF will be replaced by CRLF in .gitignore.  
The file will have its original line endings in your working directory.  
#CR:carriage return 回车，光标到首行，'\r'=return  
#LF:line feed换行，光标下移一行，'\n'=newline  
#linux:换行\n  
#windows:换行\r\n  
#MAC OS:换行\r  
#提交时转换为LF,检出时转换为CRLF,默认设置不用修改,Git是linux配置  
git config --global core.autocrlf true  
#允许提交混合换行符的文件  
git config --global core.safecrlf false  
