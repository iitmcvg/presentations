27th July, 2018

# TGIF 

Varun Sundar
 
---

## Disclaimer

* @size[x-large](You are part of privy info)

* @size[x-large](With great power comes great responsibility)

---

## Agenda Points:

1. Refining our goals
2. Work ethic
3. Semester plan
4. Inventory changes and management

---

## Section 1: Our Goals

* To create a *technically competent* community of AI and vision experimenters.

* broad goal

* each of us may have different interpretations

+++

* Need everyone to share a goal.

* Might evolve with time.

---

## Section 2: Work Ethic

* Fixed place, Fixed time

* continuous work is needed to develop expertise

+++

* Our objective will always be to improve quality

* This includes:
    - Technical expertise (optimised pipelines, more experimentation)
    - Content management
    - People management

+++

### Fixed place, Fixed time ...

- Wednesday for technical discussions 
    - frameworks/ papers
    - 1-2 hours

+++

- Fridays (or Thursdays) for admin meetings
    - Meant for all of you to keep in touch with happenings
    - Cross collab among teams working in different topics

- Full flexibility in topic otherwise.

Note:
* Not only tech topics

---

## Section 3: Semester Plan

---
 
### 3.1 Work we take up

* Projects of two kinds

    - Impactful real world projects

    - Academic oriented ones

+++

### 3.1.1 Impact projects

* Deploy to see results

* May not be as technically challenging

* Getting it to work in env is harder

* AI- 3-5/10, Engineering- 6-8/10, People- 8-9/10

+++

### 3.1.2 Academic projects

* Hallmark topics plus areas

* To improve in-house expertise

* AI- 8-9/10, Engineering- 2-3/10, People- 0-2/10

+++

* Areas : (subject to discussion)

 1. Pattern recognition, DL with associated NLP
 2. Robotic vision, Drone navigation
 3. Deep RL
 4. DL in computational photography

+++

* Can look at goals of papers plus patents, deployment.

---

### 3.1.3 Present Tie-Ups

For Impact Projects

* _Verihelp_, a startup using AI to secure school children

* A Shipping based company, which wants to automate maintainance tasks.

* Hyperverge, Predible in possiblities too

Note:
 - Why havent we named the shipping company?
 - Ask muthu XD

+++

### Testing waters

* Plan on taking up two only till December

* Have setup a SOP for external Projects

---

### 3.1.4 External Projects SOP

* Pipeline: 
    - Receive or Seek proposal
    - Literature Survey
    - POC
    - setup terms of operation, team bandwidth
    - Project

* Shipping company PS is in POC stage, Verihelp is in POC talks.

+++

* Full details: Drive/Documents/Propositions/External-Project-Template

* [Link](https://docs.google.com/document/d/1OUbwkQkI8m5wGkM7gBmytEiduPVHMGGiGutQOfMYDm0/edit?usp=sharing)

---

## 3.2 KeyStone Events

* We target (not limited to) events which could help us gain expertise

* Spread across the Semester

+++

* Aug - None (besides, intro sessions)
* Sep - Pysangamam, Pycon, DL Master class
* Oct- Open House
* Nov - .
* Dec - Tech Meet, CVG Meet?
* Jan - AI Conference

+++

Long term: AI4India

+++

## PySangamam

* 7th, 8th September.

* 3 submissions (4 people), shortlisting on 1st Aug.

* Will also be conducting a workshop (to finalise this week)

* Also 1 submission to _Pycon_

+++

## DL Masterclass (_Bootcamp?_)

* In mid September, either post 10th or post 24th.

* Need to understand pros-cons from last year, what impact we want.

* RL masterclass next sem

+++

## OpenHouse

* 3rd week of Oct (mostly)

* Handling present projects:
    - Finish till you setup optimal exeperimentation pipelines.
    - more on this in our technical meets
    - Then choose to document and move on or scale up.

+++

* Work on your theory as you build your pipelines for existing projects.

* Reduce iteration time for new topics you want to take up.

* Be good at atleast one framwork.

+++

## The Rest

* Will update in upcoming meetings

* AI Conference ideation is done, will be setting up the executing group

* CVG Meet of all our seniors. 

* Want all of you to head your own events.

* More here: [Documents/Meetings/Stakeholders-AI-Conf](https://docs.google.com/document/d/1_RVTnkloheBQVXmbjG9RO12z-QIKQEMkaR2P84HwFc0/edit?usp=sharing)

@Note:

- Communication tools: Whatsapp or slack
- Use the drive account.

---

## 3.3 Branding

@ul 

* If we are really good at what we do, we need to showcase it.
* Work on online presence.

@ulend

+++

### Online Presence

* Medium for posts. (target 3-4 a month)

* Overhaul both Fb, Twitter (pages, handles)

+++

* Seperate present blog, create a proper landing page

* Landing page has to be impressive.

* See

Note:
    - Logos, Page Banners

+++

### Handling 100 ML Days

* Worthwhile considering we want to work regularly

* Logging of our change

* Need to tell a story.

* Opinions?
---

## 3.4 Standardisation

With respect to:

* Content  
* Documentation  
* Optimised pipelines for common tasks 
(or _engines_ if you may)  
* Custom (private) Datasets

---

## Section 4: Inventory management

* 4 cameras (go pro, Logitech 270,310,922x). A. Tripod

* Pendrives

* Meta Pro glasses.

+++

* System to handle usage (TO-DO)

+++

### 4.1 Training Infra

* MSI
* Workstation

+++

Workstation Specs:

    - i7, 12 cores
    - 64 GB RAM
    - 3 GPUs ( 1 fitted currently)
    - 4Tb + 256 GB Storage

---

### 4.2 Access to GPU's

* Dockerised containers
* Mounted HOME and Media dir's (your code is saved)
* Train responsibly

+++

Access: (similar to)

`ssh -p XXXX varun@iitmcvg.local`

Port numbers are unique. User names are unique.

+++

### Training Guidelines

* Binary files on SSD (lmdb, TF Records

* Donot install cross-dependencies, ask for another container

* Keep containers with bare minimum internal libs (add to the DOCKERFILE instead)

---

### 4.3 Ways your container can die

@ul
* Fill up your allocated HDD/SSD limits

* `rm -rf` for no joy

* Use passwords for SSH (use only SSH Keys)

* Use anaconda on top of docker (_Why, just why?_)

@ulend

Wish this could be more dramatic...

+++

### Other points

@ul
* Setup your remote tools 

* Donot be heavily reliant on Desktops/ VLC

* Eg: Use rmate for vscode, or vim

@ulend

---

## Section 5: Workspace

Open for discussion

---

## Appendix

Open roles for heading:
    - Branding
    - Events (AI Conf, DL masterclass, AI4India)
    - New topics (drone navigation, DRL)
    - Impact Projects
    - Standardisation process.



