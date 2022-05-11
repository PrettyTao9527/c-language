```
Git is a distributed version control system.
Git is a distributed version control system.
Git is free software distributed under the GPL.
I'm a freshman of the git software.
I'm always confused about how to use Git well.
But would you mind giving me some help?
我够快被git的撤销修改命令整懵逼了，咋办？？？
我要疯了！
what should I do for it??

1.未add之前"git restore filename"=="git restore --worktree filename"=="git checkout -- filename";<*已验证*>
2.在add之后好像"git restore --staged filename" or "git restore filename"好像都不能撤销上一步的修改，而"git checkout -- filename"则可以，而且不管你是否有commit都可以，只要未关闭git bash here,都可以回到上次关闭bash之前最后一次add的状态。这就很尴尬了，毕竟教程的版本跟我的不一样，时代都在进步;

```