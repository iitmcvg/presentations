7th July, 2018

@snap[north-east sidebar]
![cvi](http://iitmcvg.github.io/assets/avatar.png)
@snapend

@snap[south-east sidebar]
![cfi](http://cfi.iitm.ac.in/main/wp-content/uploads/2014/09/favicon.png)
@snapend

# Git Session

Varun Sundar

---

## Topics:

@ul
1. What, why and how?  
2. Your first repo.  
3. A gist of git commands.  
4. Some more steps.  
5. Git oriented practices.  
6. Other use cases.  
@ulend

---

Section 1: 

### Git is really beautiful, well setup.

But it takes some time to get a grasp.

Feel free to shoot questions.

+++

#### This presentation was made with git!

+++

* Version tracking tool

* Distributed versioning system (more local, but can setup central systems)

* originally developed in 2005 by Linus Torvalds

* Successor to CVS (central versioning systems), Subversion (also known as SVN)

+++

![image1](https://www.techwebies.com/wp-content/uploads/2015/09/svn-repo.png)

+++

![image2](https://securityonline.info/wp-content/uploads/2017/09/centralized-vs-distributed.jpg)

+++

![image3](https://www.addteq.com/blog/files/113446998/113447001/1/1457715739000/gitvssvn.png)

+++

### Strenghts

* Performance: 
    - Committing new changes, branching, merging and comparing past versions are all optimized for performance.

* Focus on content not file names.

* Supports non-linear, scale variant development. (Branching, Merging)

+++

### Overall Picture

![Git overall](https://wac-cdn.atlassian.com/dam/jcr:2bef0bef-22bc-4485-94b9-a9422f70f11c/02%20(2)

---

### Section 2: Hello git

Let's code this along!

+++

### Step 1: Who are you (to git)?

```
git config --global user.name "Mona Lisa"
git config --global user.email "mona.lisa@da-vinci.com
```

+++

Optional Stuff

```
git config --global color.ui "auto"
git config --global core.editor "nano"
```

+++

You can display these by

```
git config --global user.name
git config --global user.email
```

+++

### Step 2: Find a directory of interest

```
cd foo
git init
```

+++

### Step 3: Add, update files

```
git add . && git add -u
```

+++

### Step 4: Add a remote

```
git remote add url
```

+++

### Step 5: Push to origin at master

```
git push --set-upstream origin master
```

I'll shortly explain what a remote, origins and master's are.

---

## Section 3: Some Git Vocab

* **Working Tree**: A directory in your filesystem with the code.

* **Repository**:A collection of commits and branches saved in the .git directory.

* **Commit**: A snapshot of your working tree, identified by the revision number.

* **HEAD**: the commit your work tree is currently at.

---

## Section 3.2 Git Config

* is a convenience function that is used to set Git configuration values on a global or local project level. 

* These configuration levels correspond to .gitconfig text files. 

* `git config --<level> <object>.<property> <attribute>`

+++

### Continued:

* Levels:
    --local (project specific)  
    --global (user specific)  
    --system (all machines)  

+++

* Some objects and properties:
    - user >> email, name  
    - merge >> tool  
    - color >> ui  
    - alias >> <name for alias >  
    eg: `git config --global alias.ci commit`  

---

## Section 3.3 Saving Changes

* git add
* git commit
* git diff
* git status
* git stash

+++

### Git add

* adds a change in the working directory to the staging area

![git add](https://www.atlassian.com/dam/jcr:0f27e004-f2f5-4890-921d-65fa77ba2774/01.svg)

+++

### Git commit

* Stages a series of edits

* Can be resetted by `git reset`

* No interaction with anything remote. 100% local.

* Record snapshots (not differences like CVS, SVNs)

+++

![staging](https://www.atlassian.com/dam/jcr:7406fe56-d36d-44cf-92e3-b28e4bae36f8/02.svg)

+++

* Commits are cheap, fast.

* Recommended to commit as much as needed.

* There's a caveat.

+++

![humour](https://camo.githubusercontent.com/9dff2ed7d6ca58a6d44d600d56658d1d5b1fa24b/687474703a2f2f696d67732e786b63642e636f6d2f636f6d6963732f6769745f636f6d6d69742e706e67)

+++

### Staging area

* buffer between the working directory and the project history.

* allows an important seperation:
    - working history
    - commit history
    - staging history

* Can commit changes logically, instead of en-masse.

+++

### How staging works

![image-staging](https://github.com/mbjoseph/git-intro/raw/master/fig/git.png)

+++

### Git Diff

* differences between two snapshots or files

* Default: diffs in previous commit

Eg:
```
git log --pretty=oneline
```

+++

#### Options ...

![git stash](https://www.atlassian.com/dam/jcr:d6fec41a-dc66-4af6-8b0f-c23d271eaf8e/01.svg)

+++

### Git stash

* Temporary stage

* Store with `git stash`

* Pop to reapply: `git stash pop` 
(remove from and make changes to dir )

`git stash apply`
(remove from and make changes to dir and stash)

---

### Git ignore

* Use regex's

* Again, can use global or local rules.

+++

### Let's try this

Introduce a big file in your dir.

```
vim .gitignore
```

+++

Add the file to ignore.


Try commiting and pushing again.

---

## Section 4: Some more baby steps

### 4.1: Branches and Merging

* Branch == Named Commit

* Default is master.

* Allows for deviations in code developement.

+++

* A branch is local to your repo

```
git checkout -b fancybranch
```

If you want to switch back to master

```
git checkout master
```

+++

Pushing to a branch

```
git push <remote> <branch>
```

eg:

```
git push origin fancybranch
```

or, (since git is smart):

```
git push
```

+++

You can delete a branch too

```
git branch -d fancybranch
```
---

### Section 4.2: Remotes (fun stuff ahead)

* Besides your local copy, a copy on a server.

* Public hosted or Private.

* Major providers:
    * Github  
    * Gitlab  
    * Bitbucket  

+++

### Github vs. GitLab vs. Bitbucket

![git-providers](https://www.amarinfotech.com/wp-content/uploads/2017/05/GitLab-vs-GitHub-vs-bitbucket-1.jpg)

+++

Popularity

* Github is the gold standard for opensource code.  
* Gitlab Enterprise for premise installs  
* Bitbucket is marginal for both  

+++

![opensource](https://content.nexosis.com/hs-fs/hubfs/posts/Stack%20Overflow%20Trends/GitHub-GitLab-Bitbucket-border.jpg?t=1535133708722&width=612&height=437&name=GitHub-GitLab-Bitbucket-border.jpg)

+++

![self-host](https://user-images.githubusercontent.com/4660275/34914739-d929d7dc-f929-11e7-945f-daf17005a767.png)

+++

Private repos:

* free on Bitbucket (w/ < 6 collaborators)  
* free on GitLab (unlimited collaborators)  
* not free on Github  
---

### Section 5: Git Oriented Practices (Optional)

* Seperate master and develop branches

* Use a wrapper called `git flow`

* Generic syntax : `git flow <type of branch> <start/finish> name`

+++

### Dev vs Master

![git flow features](https://www.atlassian.com/dam/jcr:b5259cce-6245-49f2-b89b-9871f9ee3fa4/03%20(2).svg)

`git flow feature start feature_branch`

`git flow feature finish feature_branch`

+++

### Release, Bug fixes

![Git release, bug fixes](https://www.atlassian.com/dam/jcr:61ccc620-5249-4338-be66-94d563f2843c/05%20(2).svg)

* release: a soft dev term; comprises docs, containers, release features

* once released, you merge it into master and dev

```
git checkout master  
git checkout merge release/0.1.0  
git flow release finish '0.1.0'  
```
---

### Section 5.2 : Dealing with Large Bianries 

@ul
* Large binaries are often issues in version control  

* How big? Say > 10 MB, binaries.

* Code not an issue

@ulend

+++

@ul

* Git doesnt track them line wise

* So for every minor mod, you incurr a big penalty

* 50 MB >> 100 MB >> 150 MB, blows up soon

@ulend

+++

### Dealing with Large Binaries

@ul
* Dont add them !

* Git solutions:
    * Git LFS >> Too slow
@ulend

+++

### Our recent approach

* Adding binaries with a seperate tag.

* We don't track them, just sync

* Syncs to a common HDD.

* No change in workflow for dev, except 

`foo/bar.b` becomes `lazydata(track('foo/bar.b'))`

---

## Section 6: Other Use cases

* You can tie your entire workflow to git.

* Details, discussion offline.

+++

### That's all for now !
### Any question?
### Slides available at : https://gitpitch.com/iitmcvg/presentations/master?p=git-session#/5

---