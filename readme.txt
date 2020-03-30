回退的问题：
1）工作区文件回退到暂存区的文件，还未git add，直接用git checkout -- <filename>即可；
2）工作区文件回退到暂存区的文件，但已经git add还未commit，用git restore -- stage <filename>或者git reset HEAD <filename>将暂存区文件恢复到上一个commit的版本，再用1）中的git checkout -- <filename>将暂存区文件恢复到工作区；
3）已经commit的文件回退，参考版本回退，git reset --hard HEAD^直接将上一个版本的代码退回到暂存区和工作区。ps：此处不用再做2）和1）中的操作，因此需特别小心！
ps：有没有可能只回退某个文件而非整个版本？
adding a new branch
just here
