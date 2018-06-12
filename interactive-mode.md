### git add -i 进入互动模式下的8个命令

**Commands**

  1: status       2: update       3: revert       4: add untracked
  
  5: patch        6: diff         7: quit         8: help
  
**命令介绍**
* status
  > 查看版本库、暂存区、工作空间之间的变化

  >sample:![status](status.png)

  >根据图示，readme.txt版本库和暂存区之间是一致的，暂存区和工作空间之间有区别

* update
  > 进入如下命令窗口：

  >![update](update.png)

  >可以输入指定行号用以选中，输入形式可以是 1 2,3 3-5 7-
  >
  >被选中的行左边会有个 * 号
  >
  >之后输入空命令（直接回车）被选中的文件会被加入暂存区

* revert
>可以将选中的文件退回到HEAD版本。操作方式类似于update

* add untracked
>可以将新文件加入到暂存区。操作方式类似于update，revert

* patch
>选中的文件会依次展示其变更，并提供如下一些命令来使用
- y - stage this hunk
- n - do not stage this hunk
- q - quit; do not stage this hunk or any of the remaining ones
- a - stage this hunk and all later hunks in the file
- d - do not stage this hunk or any of the later hunks in the file
- g - select a hunk to go to
- / - search for a hunk matching the given regex
- j - leave this hunk undecided, see next undecided hunk
- J - leave this hunk undecided, see next hunk
- k - leave this hunk undecided, see previous undecided hunk
- K - leave this hunk undecided, see previous hunk
- s - split the current hunk into smaller hunks
- e - manually edit the current hunk
- ? - print help
