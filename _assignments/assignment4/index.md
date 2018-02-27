---
layout: base/bar/bar-sidebar-none
title: "Assignment 4: Communicating Your Design"

due_project_4a: Uploaded Monday (due night before class), March 5, 2018
link_project_4a: https://canvas.uw.edu/courses/1124153/assignments/3986574

due_project_4b: Uploaded Wednesday (due night before class), March 7, 2018
link_project_4b: https://canvas.uw.edu/courses/1124153/assignments/3986575

due_project_4c: Completed in section on Friday, March 9, 2018

due_project_4d: Uploaded Friday, March 9, 2018
link_project_4d_poster: https://canvas.uw.edu/courses/1124153/assignments/3986577
#link_project_4d_video: https://canvas.uw.edu/courses/1098203/assignments/3615348

due_project_4e: Attend 10:30am-12:30pm, Monday, March 12, 2018

---

<div class="alert alert-danger" markdown="1">
This page is still being migrated and developed.
Information here is likely suggestive of the final page, but remains subject to change.
</div>


# Overview

You have identified a problem, explored a design space, selected a promising design, and iterated on that design.
It is now time to focus on communicating your design and your design process.
This group assignment communicates your design through a __website__, a __poster__, and a __pitch__.

This assignment is worth __15 out of 100 points__ of your overall course grade:

- __5 points__ for the milestones 
  - __3 points__ for [Assignment 4a: Initial Website](#initial_website)
  - __2 point__ for [Assignment 4b: Poster Critique and Pitch](#poster_pitch)
- __5 points__ for [Assignment 4d: Final Website](#final_everything)
- __5 points__ for [Assignment 4d: Final Poster](#final_everything)

[Assignment 4e: Poster Session](#poster_session) is intentionally not graded.

# Milestones

This is a group assignment, consisting of six milestones.

* [Assignment 4a: Initial Website](#initial_website)

  Due: {{ page.due_project_4a }}

* [Assignment 4b: Poster Critique and Pitch](#poster_pitch)

  Due: {{ page.due_project_4b }}

* [Assignment 4c: Communication Critique](#communication_critique)

  Due: {{ page.due_project_4c }}

* [Assignment 4d: Final Poster and Final Website](#final_everything)

  Due: {{ page.due_project_4d }} 

* [Assignment 4e: Poster Session](#poster_session)

  Due: {{ page.due_project_4e }}

# Project Description

In this assignment, you communicate your design in several forms.
You will create a website, a poster, and a pitch to present your work from the entire quarter.

1. Create a project website that provides an overview of the project, 
   presents your design process, and introduces team members. 
   At a minimum, it must include links to your 
   [Assignment 2]({{ site.baseurl }}/assignments/assignment2/) report, 
   your [Assignment 3]({{ site.baseurl }}/assignments/assignment3/) report, and your poster.
   Optionally, also include your presentations or other materials.
   Ideally, much of this same content will also be presented in a manner more appropriate for the web. 
   
   Be sure you have updated any documents that course staff said needed fixed before posting 
   (e.g., any report that accidentally included participant identifying information). 

2. Create a poster that communicates your design and your design process to a general audience.
   The goal is to present your work in a visual form to interested parties from across campus or from industry. 
   You need to quickly convey the most important aspects of your work. 
   The poster must be 32"x40" (portrait, vertical). 
   
3. Create a pitch that you can deliver together with your poster.
   This should summarize the problem and your design.
   It should be no more than 1 minute long.
   This pitch should convince the audience your problem was worth investigating and that your design effectively addresses it.

# Deliverables

<a name="initial_website"></a>

## 4a: Initial Website

Due: {{ page.due_project_4a }}

We will use your websites to advertise the poster session.
Although this is in an initial website on which you will get feedback and will be able to update,
you should submit a complete and high-quality versions of your website.

Your website will be served from a subdirectory of this course website.
It is also link via a thumbnail from the projects page:

[Projects Page]({{ site.baseurl }}/projects.html)

You can build your website however you like, but everything needed for your site must be in your directory.
Do not attempt to integrate with the Jekyll functionality used for this course website.
Simply build your website and submit the set of static files to be served from your directory. 

### Samples from Prior Offerings

Samples from prior offerings include:

{% for currentoffering in site.data.samples.offering %}{% for currentsample in site.data.samples[currentoffering.key] %}
  -  {{ currentoffering.name }} - [{{ currentsample.name }}]({{ currentsample.link }}){% endfor %}{% endfor %}
  
Note that details of assignments may have changed since prior offerings, so their reports may not map to the current project.
Also note these samples are intended to illustrate a variety of approaches, none of which is intended to be ideal or exemplary.
Be sure to understand and carefully consider project requirements and feedback from the course staff in the context of your own work.

### Submission

Github repo: https://github.com/uwcse440/web-cse440-wi18

Submit a pull request containing your website. We will merge as quickly as possible. 
You can submit multiple requests as needed to fix issues or improve your website.
Your request should not modify anything outside your project website.

Submit simple pull requests early so that you become familiar with this functionality.
Do not wait until the final moments to begin to learn how to do this.

If you are absolutely unable to submit a pull request, submit via Canvas here:

{% if page.link_project_4a != nil %}<{{ page.link_project_4a }}>{% else %}`Link to be added`{% endif %}

### Grading

This milestone will be graded on a scale of __3 points__:

1.  __Completeness of Content__: (1 point)
2.  __Appropriately Polished Presentation__: (1 point)
3.  __Submitted via Pull Request__: (1 point)

Your website should be complete and will be evaluated as such.
But later critique and refinement will help further improve it before the final poster session.


<a name="poster_pitch"></a>

## 4b: Poster Critique and Pitch

Due: {{ page.due_project_4b }}

Your poster should include:

- Logo
- Project Title
- Your Names
- Problem
- Value Proposition
- Key Functionality
- Design Process and Iteration

Your poster should include images and limited amounts of text.

An effective poster size is 32"x40". A PowerPoint template is available here:

[Cow Project PowerPoint template]({{ site.baseurl }}/samples/4c/poster_template.ppt)

You should heavily modify the template to be unique and represent your project.

During the final poster session, your team will give a one minute pitch to a small group of judges. 

Be prepared to give this pitch in class and when presenting the poster.
Course staff and other students will give feedback so you can improve before the final poster session.

### Samples from Prior Offerings

Samples from prior offerings include:

{% for currentoffering in site.data.samples.offering %}{% for currentsample in site.data.samples[currentoffering.key] %}
  -  {{ currentoffering.name }} - [{{ currentsample.name }}]({{ currentsample.link }}): [4c_{{ currentsample.suffix }}.pdf]({{ site.baseurl }}/samples/4c/4c_{{ currentsample.suffix }}.pdf){% endfor %}{% endfor %}

Note that details of assignments may have changed since prior offerings, so their reports may not map to the current project.
Also note these samples are intended to illustrate a variety of approaches, none of which is intended to be ideal or exemplary.
Be sure to understand and carefully consider project requirements and feedback from the course staff in the context of your own work.

### Submission

Submit your poster via Canvas here: 

{% if page.link_project_4b != nil %}<{{ page.link_project_4b }}>{% else %}`Link to be added`{% endif %}

Your poster may be in PPT, PPTX, or PDF format. 
We have a color plotter that can print posters this size. 
Your source file is due as above, we will then coordinate with you for proofreading and printing.

Be prepared to give your elevator pitch in class.

### Grading

This milestone will be graded on a scale of __2 points__:

1.  __Initial Poster__: (1 point)
2.  __Initial Pitch__: (1 point)

<a name="communication_critique"></a>

## 4c: Communication Critique

Due: {{ page.due_project_4c }}

This is a flexible critique day. 
The purpose of this day is to help you refine whichever of your remaining deliverables you feel needs feedback. 
Be prepared to present your website and/or poster at the critique. 
This is the last opportunity for you to get in-class critical feedback, so use it wisely.

### Submission

Bring at least one of your artifacts to class (e.g., be prepared to show them on a laptop).

<a name="final_everything"></a>

## 4d: Final Poster and Final Website

Due: {{ page.due_project_4d }} 

Course staff need your finalized poster as soon as possible, to organize printing and preparing for the poster session.

Finalize your website so we can finalize grading.

### Submission

Submit your final poster as soon as possible here:

Poster: {% if page.link_project_4d_poster != nil %}<{{ page.link_project_4d_poster }}>{% else %}`Link to be added`{% endif %}

Submit a pull request containing your website. We will merge as quickly as possible. 
You can submit multiple requests if needed to fix issues or improve your website.
Your request should not modify anything outside your project website.

Submit simple pull requests early so that you become familiar with this functionality.
Do not wait until the final moments to begin to learn how to do this.

<!-- Depending on how you embed your video in your website, it may or may not be part of the pull request.
For example, embedding a YouTube or Vimeo player does not give us your video.
We therefore explicitly ask that final videos also be submitted via Canvas here: 

#Video: {% if page.link_project_4d_video != nil %}<{{ page.link_project_4d_video }}>{% else %}`Link to be added`{% endif %} -->

### Grading

Your final website and final poster will each be graded on a scale of __5 points__.

#### Poster

- __Content__: (2.5 points)
  - Includes all of the points listed in 4b "You poster should include: ..."
  - Key features of the design are clear
  - Gives insight into the design process
- __Presentation__: (2.5 points)
  - Large images that show the key parts of the design
  - Only minimal and appropriate use of text
  - Text is large and legible
  - Colors and fonts are a pleasing combination and easy to read


#### Website

- __Content__: (2.5 points)
  - Includes all of the points listed in 4b "You poster should include: ..."
  - Key features of the design are clear
  - Gives insight into the design process
  - Links to your reports
- __Presentation__: (2.5 points)
  - Looks professional and is something you would consider including in a design portfolio

<a name="poster_session"></a>

## 4e: Poster Session

Attend {{ page.due_project_4e }}.

Come to the poster session to show off your work and engage with your classmates.
Present your pitch to a team of judges.

We will not be conducting any evaluation at the poster session itself. 
Take the opportunity to present your work, chat with judges,
engage with other students, and reflect on a busy and productive quarter.
