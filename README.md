## What I did in this repo?
This is a markdown only repo for my git learning experience. I will write down what Git command have excuted at first, then explain where and why I did it. All the document written by Vim. Hope you git beginner can also learn how to use Git by watch what I have down. Don`t hestate to tell me new things and point out what I did wrong. I would be really appreciate it.

If you are curious about why I write this README in English after you find out actually my native language is Chinese. Well, the truth is I JUST WANT.

---

## Where to learn git
I have tried to learn git a lot of times. But everytime I finish the basic, I will forget after few days without practice it. Here is some great website lying in my bookmark may help you learn.

- [Missing Semester-Git](https://missing.csail.mit.edu/2020/version-control/)
- [Learn git branching](https://learngitbranching.js.org/?demo=&locale=zh_CN)
- [CS Visualized:Useful Git Commands](https://dev.to/lydiahallie/cs-visualized-useful-git-commands-37p1)
- [Oh Shit, Git](https://ohshitgit.com/#change-last-commit-message)

---

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

---

I need to take a break today after doing my paper work. See you soon~

- `git add README.md`: Same as before.
- `git commit -m 'tired day & commit my words'`: boring commit, but concise.
- `git push`: This will automate push to my master branch.

---

I add few website that's really great to learn git. And We are going to something new now.
- `git branch feature`: Branch is a really important idea in Git, 'feature' is just a name I call this branch. Programmers are not always working on only one same feature all, so they created the 'branch' thing. You can image 'master' or 'main' anyway as main road, and there are many other road connected with main road, we call this as 'branch'. And you need to name it! hhhhhh
  ![](https://github-ihs-1257225145.cos.ap-shanghai.myqcloud.com/picgo/git-branch.png)

- `git checkout feature`: After you create the branch, you need always be cautious about which branch you work on, in case you make a mess. Now You are in a new branch (the yellow road). You can also create a new branch based on branch, there is no problem.

- `git add README.md`: Same thing as before.

- `git commit -m 'add new branch'`: Same commit as before.

- `git push`: Same push as before but on 'feature' branch. Later we will figure out how to deal with this branch.
  When I try to push this to my repo, I came across a `fatal` which says,

  ```shell
  fatal: The current branch feature has no upstream branch.
  To push the current branch and set the remote as upstream, use
  
  					git push --set-upstream origin feature
  ```

- `git commit --amend --no-edit`: Well, I find out that the little mistake alrealy be 'commit'ted , so I followed the tips in [Oh Shit, Git](https://ohshitgit.com/#change-last-commit-message).
- `git push --set-upstream origin feature`: It`s very clear that we don't have branch on our remote repo. I follow the hint and  things goes fine. Such a relief!

