PySangamam

# Engineering documentation for scientific python

_Varun Sundar_
_Draft Slides, 20th July 2018_

---

## Disclaimer

* Most of this presentation is with scientific python use cases as an instance

* May be more generally applicable. 

* Encouraged to fork out your own inference of this !

---

## The Problem at hand

Well good documentation is an utopian concept.

Does it even exist?

+++

We all know how crucial documentation can be.

Do we?

---

## Caution : Numbers ahead!

* Stack overflow developer survey 2016

* An annual survey of developer practices, issues, popular opinions 
_(tabs vs spaces anyone?)_

* ![Challenges-at-work](pysangamam/varun/stackoverflow-challenges-2016.png)

+++

* Comes in at no 2

* Poor docs or inexistent docs or inconsistent docs

* no's 1,3 are related to communication too

---

## Why are some docs bad?

* Most reasons >> docs don't give you what you _actually_ need.

* sort of like this...

* ![bridge-out-ahead](https://i.imgflip.com/20tthj.jpg)

+++

## Or...

* Docs are out of date.

* Obsolete docs can be more harmful than no docs.

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

* keep only content on source repo's

* no style sheets, index files on source repo's

---

## Appendix





