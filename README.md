## What I did in this repo?
This is a markdown only repo for my git learning experience. I will write down what Git command have excuted at first, then explain where and why I did it. All the document written by Vim. Hope you git beginner can also learn how to use Git by watch what I have down. Don`t hestate to tell me new things and point out what I did wrong. I would be really appreciate it.

If you are curious about why I write this README in English after you find out actually my native language is Chinese. Well, the truth is I JUST WANT.

## What I did?
- `git init`: Create a repo folder under where you put your code, then `git init` in Terminal under this folder. You will see a `.git` file be created. If not, check what the hint says. The `.git` file track what you have done under this folder, which is the most important thing - version control, and it will be hidden unless you use `la` in Unix-like terminal or show hidden file. 
- `vi README.md`: All the things written by now in this markdown.
- `git add README.md`: Actually the file will not be tracked if you don't add them. If yout want track all the code file under this folder, you  may need `git add .` Instead of track specific one.
- `git commit -m 'init repo & add readme'`:  Well, you can think about this command this way. You got a homework and finished it. But at this time, only yourself know you have done it. After you tell(commit) your mom(`.git`) you did, She will let you go.
- `git remote add origin https://github.com/hanwinbi/git-experience.git`: Create a repo in your Github account or other platform place your code when you want to share it or cooperate with others. You can also only do version control on local.
- `git branch -M master`: This is the first time use `-M` parameter. It's a shortcut for two params `--move --force`, which means rename the branch even if the new branch name already exists. Ref: [Git - git-branch Documentation (git-scm.com)](https://git-scm.com/docs/git-branch)
- `git push -u origin master`: This will push all your added local file to Github. Ohhhhhh~
- `git add README.md`: I need to add this to track what I did after last `add`.
- `git commit -m 'add remote repo & push'`: Same things as before, but different commit message.
