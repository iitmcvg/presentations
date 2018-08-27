## Infra Setup 

Covers the starter pack for using our infra setup.

---
## Philosophy

@ul

* Common workflow for everyone irrespective of hardware.
* Common shared fixes and working code.
* Common shared resources which is version controlled.
* Hassle free ways to present our work and maintain a portfolio.

@ulend
---
## How we did it?

One word:

**Git**

---

* Everything is tied to only one version control system.

* You are used to it, not another hassle.

---

* We keep our github clean.

* New features are added as external agents.

---

## The solutions

1. Common workflow: Containers with code on github.
2. Intra-team Docs: G3Docs
3. Portfolio: Github pages
4. Formal Docs: LaTex with git (Overleaf)

---

## The only price to pay ...

* A common workflow 

```
--g3docs/
    --folder1/
--dockers/
    --foldera/
    --i-hate-cmake/
--papers/
   --subtopics/
-- etc/
  -- random-stuff.jpg
--src/
    -- checkpoints/
    -- codebase/
    -- log/
    -- out/
    -- script1.py
    -- script2.py
--formal_docs/
-- README.md
```

---

@ul 
* `etc`: could include your brainstorming, etc
* `g3docs` pulled to docs engine
* set script paths (PYTHONPATHS,PATHS,LD_PATHS) to base (repo)
@ulend

---

## Specifics

### Containers:

* NGC (NVIDIA CLoud Registry):
    - Built for HPC, Deep Learning, Ansys.
    - Optimised for `Pascal`, `Volta`

![image](https://www.nvidia.com/content/dam/en-zz/Solutions/cloud/ngc-gpu-cloud-diagram-625-t.png)

---

@ul 
* Has source optimised versions of all major frameworks.
* We build dockerfiles on these
@ulend

See : github.com/iitmcvg/workflow

---

* A few Dockerfiles.

---

## What after?

* We build em
* We run em

---

## Container Philosophy

* We give each of you tf and a few other standard stuff.
* Ask for specific container for crazy installs.

---

## G3Docs

* Pulls each repo's markdown files from g3docs
* Renders it in a human readable manner.

---

## Current Features

* 

---

* We are adding a few more features soon:
    - direct opening in github

---
