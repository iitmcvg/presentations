7th July, 2018

# Git Session

---

## Topics:

@ul
1. What, why and how?
2. Your first repo.
3. A gist of git commands.
4. Git oriented practices.
5. Other use cases.
@ulend

---

Section 1: 

## Git is really beautiful, well setup.

But it takes some time to get a grasp.

Feel free to shoot questions.

+++

* Version tracking tool

* Distributed versioning system (more local, but can setup central systems)

* originally developed in 2005 by Linus Torvalds

* Successor to CVS (central versioning systems), Subversion (also known as SVN)

+++



---

## Strenghts

* Performance: 
    - Committing new changes, branching, merging and comparing past versions are all optimized for performance.

* Focus on content not file names.

* Supports non-linear, scale variant development. (Branching, Merging)

---

## Overall Picture

![Git overall](https://wac-cdn.atlassian.com/dam/jcr:2bef0bef-22bc-4485-94b9-a9422f70f11c/02%20(2).svg)

---

## Section 1.1 Initialising a repo

```
cd foo
git init
git add . && git add -u
git commit -m "Initial commit"
git remote add origin <my origin>
git push --set-upstream origin master
```

---

## Section 1.2 Git Config

* is a convenience function that is used to set Git configuration values on a global or local project level. 

* These configuration levels correspond to .gitconfig text files. 

* `git config --<level> <object>.<property> <attribute>`

+++

### Continued:

* Levels:
    --local (project specific)
    --global (user specific)
    --system (all machines)

* Some objects and properties:
    - user >> email, name
    - merge >> tool
    - color >> ui
    - alias >> <name for alias >
    eg: `git config --global alias.ci commit`

---

## Section 1.3 Saving Changes

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

![staging](https://www.atlassian.com/dam/jcr:7406fe56-d36d-44cf-92e3-b28e4bae36f8/02.svg)

+++

### Staging area

* buffer between the working directory and the project history.

* allows an important seperation:
    - working history
    - commit history
    - staging history

* Can commit changes logically, instead of en-masse.

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

---

## Section 1.4 Organising this

* Seperate master and develop branches

* Use a wrapper called `git flow`

* Generic syntax : `git flow <type of branch> <start/finish> name`

---

## Dev vs Master

![git flow features](https://www.atlassian.com/dam/jcr:b5259cce-6245-49f2-b89b-9871f9ee3fa4/03%20(2).svg)

`git flow feature start feature_branch`

`git flow feature finish feature_branch`

---

## Release, Bug fixes

![Git release, bug fixes](https://www.atlassian.com/dam/jcr:61ccc620-5249-4338-be66-94d563f2843c/05%20(2).svg)

* release: a soft dev term; comprises docs, containers, release features

* once released, you merge it into master and dev

```
git checkout master
git checkout merge release/0.1.0
git flow release finish '0.1.0'
```
---

## Section 2: Our Workstation

* Acessing containers

`ssh -p XXXX name@IP`

* Any wifi in insti directly connected to insti LAN

* 10.21.XX.XX IP

+++

## Some changes you should do

* Change password, move to SSH Keys

* Add zsh flavours

* Add tmux, net-tools

---

## Section 3: Docker 

* What is docker

![docker](https://www.docker.com/sites/default/files/Container%402x.png)

---

![another image](https://docs.docker.com/engine/images/architecture.svg)

---

## The basic workflow

* Images

* Containers

* Build directives

+++

* Build>> converts a list of instructions into an image

* Image >> Serves as "OS" for various containers

---