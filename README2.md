# gitの使い方

# インストール
https://git-scm.com/install 

### Git for Windows 


### clone 時に key 指定
- 基本
  
`git -c core.sshCommand="ssh -i key/file/path/YOUR_SSH_PRIVATE_KEY" clone git@TARGET_REPOS.git`
- Git Bash (win)
  
`git -c core.sshCommand="ssh -i /drive_letter/key/file/path/YOUR_SSH_PRIVATE_KEY" clone git@TARGET_REPOS.git`

### ssh 鍵 生成

`ssh-keygen -f file/path -C "コメント"`

file/path.pub を管理者へ提出

file/path は自分以外に漏らさないように

