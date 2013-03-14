```bash
git config --global alias.co "checkout"
git config --global alias.ds "diff --staged"
git config --global alias.st "status -sb"
git config --global alias.amend "commit --amend -C HEAD"
git config --global alias.undo "reset --soft HEAD^"
git config --global alias.standup "log --since '1 day ago' --oneline --author timo.strotmann@gmail.com"
git config --global alias.graph "log --graph --pretty=format':%C(yellow)%h%Cblue%d%Creset %s %C(white) %an, %ar%Creset'"
git config --global alias.ls "log --pretty=format:'%C(yellow)%h %C(blue)%ad%C(red)%d %C(reset)%s%C(green) [%cn]' --decorate --date=short"
git config --global alias.nomerged "branch -a --no-merged"
git config --global alias.nopushed "log --branches --not --remotes --simplify-by-decoration --decorate --oneline"
git config --global alias.this "!git init && git add . && git commit -m 'Initial commit'
```
