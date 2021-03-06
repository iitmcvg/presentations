PySangamam

## Engineering documentation for scientific python

_Varun Sundar_  
_Draft Slides, 20th July 2018_

---

## Disclaimer

* Most of this presentation is with scientific python use cases as an instance

* May be more generally applicable. 

* Encouraged to fork out your own inference of this !

---

## The Problem at hand

@ul

- Well good documentation is an utopian concept.

- Does it even exist?

@ulend

+++

@ul

We all know how crucial documentation can be.

But the scale can be suprising at times.

@ulend

---

## Caution : Numbers ahead!

@ul

* Stack overflow developer survey 2016

* An annual survey of developer practices, issues, popular opinions 
_(tabs vs spaces anyone?)_

@ulend

Note:

- Using 2016, since 2017 and 2018 donot contain relevant parameters

+++

![stack-overflow](assets/stackoverflow-challenges-2016.png)

+++

@ul

* Documentation comes in at no 2

* Poor docs or inexistent docs or inconsistent docs

* no's 1,3 are related to communication too

@ulend

---

## Why are some docs bad?

* Most reasons >> docs don't give you what you _actually_ need.

+++

@ul

* sort of like this...

* ![bridge-out-ahead](https://i.imgflip.com/20tthj.jpg)

@ulend

+++

## Or...

@ul

* Docs are out of date.

* Obsolete docs can be more harmful than no docs.

@ulend
---

## Bad Docs

Hurts :

* Reliability and reproducability of code
* Slows down OSS usage

+++

## Scientific use cases

* Even more important

* Many more updates in code

* Apparent age scale has dropped >> Quicker dev cycles.

---

## Let's step back up a bit

* Documentation is everybody's problem

+++

Good Documetation could use :

* a cultural change (bottoms up approach)
* a tooling change (top down approach)

+++

## But 

* Both inflict help

* _yes, that's an oxymoron_

---

## Existing Documentation Engines 

in Python

* Sphinx

* Doxygen: tool of choice for C/C++. Not really nice with python.

+++

## Issues

* Sphinx: 

* Doxygen: Doesn't follow with 

---

## Dynamic and Integrated Docs

* What if we could integrate docs into workflow

* Build on Git's README culture.

* Much better than using wiki's.

---

## Inspiration here: G3Docs

* An internal format followed by many OSS projects in google (eg: tensorflow)

* Started when google engineers cited docs as #1 productivity issue (Googlegeist
2014)

+++

## No this isn't a google commercial

---

## The Idea

* Either auto-render or write specific docs in a determined folder on your repo

* Render these as static sites 

* Either per repo or sweep through a list.

+++

* seperate presentation from the content

* keep only content on source repo's

* no style sheets, index files on source repo's

---

## Great how do we do it?

* Generate the markdown 

* Serve the markdown

---

## Generating the markdown

@ul
Generally two requierements,

* Overall pipeline documentation

* module specific API style docs 

@ulend

+++

## Module Specific Docs

@ul
* Needs a convention

* We choose to adpot numpy convention

@ulend

+++

## Numpy convention

* Use docstrings for every :
    - module (top of the file)
    - class
    - functions 

+++

### Module documentation

* State description, example command, all possible arguments.

+++

```
'''
Foo/bar.py

To allow for better scripts

Example usage:

python root_dir/Foo/bar.py \
--flag1 arg1 \
--flag2 args

Args:

* arg1:
* arg2:
'''

import XYZ
```

+++

* Recommended execution at root of repo

* Use __init__.py files if necessary for modules

---

## Generating automatic API docs

* Pydocs if you prefer a library

* Not hard to write a custom markdown extractor

---

## PyDocs


---

## Custom Markdown Extractor

---

## Serving the Docs

Many choices:

* Mkdocs: A standard for many markdown files.

* Docsify: Has a minimal, clean interface

+++

* Besides this you could use any static site generator like:
    - Jeykll
    - Hugo

---

## Using Docsify

Structure:



---

## Appendix





