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

2.在add之后，有两种方法可以撤销上一次的修改：
①"git restore --staged filename"从暂存区回退到工作去，那么此时执行git status会发现已经没有添加的修改等待提交（no changes added to commit),然而此时只是会退到工作区，但没有删除工作区的修改，所以还要执行"git restore filename" 方能彻底撤销修改！
②"git reset HEAD filename"把暂存区的修改撤销（相当于unstaged）,此时同样是回到工作区而已，并未删除修改，需再执行"git checkout -- filename",此时才算完成撤销上次修改。

3.在commit之后，又如何撤销修改呢？方法①：版本回退命令 "git reset --hard <commit_id>" or "git reset --hard HEAD^";<*已验证*>

```