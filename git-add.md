**git add**

* -n, --dry-run 模拟add，不会真正提交。可以用来查看要提交的文件是否存在、被忽略等等。
* -v, --verbose add时会显示add了哪些文件到暂存区
* -f, --force 能够添加被ignore的文件到暂存区
* -i, --interactive 进入互动模式，会进入一个子对话窗口，有8个命令可以在该窗口执行,[查看8个命令](https://github.com/wjy030/git-ler/blob/master/interactive-mode.md)
* -p，--patch 相当于直接进入-i 中的patch命令
* -e, --edit 直接编辑变更，并将编辑结果加入暂存区（工作空间的文件不会被这次编辑修改）
* -u, --update 暂存区的文件在工作空间又被更新后，可以用-u刷入暂存区。暂存区没有的文件不会新增进来
* -A, --all, --no-ignore-removal 将工作空间指定文件的变更刷入暂存区。
* --no-all, --ignore-removal 将工作空间指定文件的变更刷入暂存区。忽略那些在工作空间被删除的文件
* -N, --intent-to-add 新增的文件无法通过git diff查看变更，执行了git add -N filename 以后就可以查看了
* --refresh
* --ignore-errors 提交暂存时忽略error
* --ignore-missing 只能和--dry-run 并用，可以查看到还未被版本管理的文件
* --no-warn-embedded-repo 
* --renormalize 强制将所有被版本管理的文件重新刷入暂存区，（This is useful after changing core.autocrlf configuration or the text attribute in order to correct files added with wrong CRLF/LF line endings. ）该方法包含了一个-u
* --chmod=(+|-)x
* -- 当命令和文件名有冲突时，用此隔离命令与文件列表
