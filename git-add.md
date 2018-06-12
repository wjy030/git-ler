**git add**

* -n, --dry-run 模拟add，不会真正提交。可以用来查看要提交的文件是否存在、被忽略等等。
* -v, --verbose add时会显示add了哪些文件到暂存区
* -f, --force 能够添加被ignore的文件到暂存区
* -i, --interactive 进入互动模式，会进入一个子对话窗口，有8个命令可以在该窗口执行,[查看8个命令](https://github.com/wjy030/git-ler/blob/master/interactive-mode.md)
* -p，--patch 相当于直接进入-i 中的patch命令
* -e, --edit 直接编辑变更，并将编辑结果加入暂存区（工作空间的文件不会被这次编辑修改）
