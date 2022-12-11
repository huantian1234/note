ssh -T git@github.com出现需要输入密码,输入之后提示Permission denied, please try again.


测试HTTPS端口ssh是否可行:ssh -T -p 443 git@ssh.github.com

编辑~/.ssh/config
```
Host github.com
Hostname ssh.github.com
Port 443
User git
```
