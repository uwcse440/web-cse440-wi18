---
layout: base/bar/bar-sidebar-none
title: "Assignment 4: Communicating Your Design"

due_project_4a: Uploaded Monday, November 27, 2017
link_project_4a: https://canvas.uw.edu/courses/1173784/assignments/3960517

due_project_4b: Uploaded Monday, December 4, 2017 (before class on Tuesday, December 5, 2017)
link_project_4b: https://canvas.uw.edu/courses/1173784/assignments/3960518

due_project_4c: Uploaded Wednesday, December 6, 2017 (before class on Thursday, December 7, 2017)
link_project_4c: https://canvas.uw.edu/courses/1173784/assignments/3960519

due_project_4d: Completed in section on Friday, December 8, 2017

due_project_4e: Uploaded Monday, December 11, 2017
link_project_4e_poster: https://canvas.uw.edu/courses/1173784/assignments/3960521
link_project_4e_video: https://canvas.uw.edu/courses/1173784/assignments/3960522

due_project_4f: Submitted Monday December 12, 2017

due_project_4g: Attend 11:00 to 12:20, Thursday, December 14, 2017

---

<div class="alert alert-danger" markdown="1">
This page is still being migrated and developed. All content remains subject to change.
</div>

# Overview

You have identified a problem, explored a design space, selected a promising design, and iterated on that design.
It is now time to focus on communicating your design and your design process.
This group assignment communicates your design through a __website__, 
a __video prototype__, a __poster__, and a __pitch__.

This assignment is worth __15%__ of your overall course grade:

- __4%__ for [Assignment 4e: Final Video Prototype](#final_everything)
- __4%__ for [Assignment 4e: Final Website](#final_everything)
- __4%__ for [Assignment 4e: Final Poster](#final_everything)
- __3%__ for the milestones 
  - __1%__ for [Assignment 4a: Initial Website](#initial_website)
  - __1%__ for [Assignment 4b: Initial Video Prototype](#initial_video_prototype)
  - __1%__ for [Assignment 4c: Poster Critique and Pitch](#poster_pitch) 

[Assignment 4d: Communication Critique](#communication_critique) and 
[Assignment 4f: Poster Session](#poster_session) are intentionally not graded.

# Milestones

This is a group assignment, consisting of six milestones.

* [Assignment 4a: Initial Website](#initial_website)

  Due: {{ page.due_project_4a }}

* [Assignment 4b: Initial Video Prototype](#initial_video_prototype)

  Due: {{ page.due_project_4b }}

* [Assignment 4c: Poster Critique and Pitch](#poster_pitch)

  Due: {{ page.due_project_4c }}

* [Assignment 4d: Communication Critique](#communication_critique)

  Due: {{ page.due_project_4d }}

* [Assignment 4e: Final Poster, Final Video, Final Website](#final_everything)

  Due: {{ page.due_project_4e }} 

* [Assignment 4f: Team Peer Feedback](#team_peer_feedback)

  Due: {{ page.due_project_4g }}

* [Assignment 4g: Poster Session](#poster_session)

  Due: {{ page.due_project_4g }}

# Project Description

In this assignment, you communicate your design in several forms.
You will create a website, a video prototype, a poster, and a pitch to present your work from the entire quarter.

1. Create a project website that provides an overview of the project, 
   presents your design process, and introduces team members. 
   At a minimum, it must include links to your 
   [Assignment 2]({{ site.baseurl }}/assignments/assignment2/) report, 
   your [Assignment 3]({{ site.baseurl }}/assignments/assignment3/) report, your video prototype, and your poster.
   Optionally, also include your presentations or other materials.
   Ideally, much of this same content will also be presented in a manner more appropriate for the web. 
   
   Be sure you have updated any documents that course staff said needed fixed before posting 
   (e.g., any report that accidentally included participant identifying information). 

2. Create a video prototype that illustrates your proposed design. 
   Use the storyboards you created as a basis for your video prototype. 
   Be sure you video conveys all of:
   
   - the problem
   - the design
   - the context 
   - the satisfaction
   
   Refer to the examples provided in lecture, as well as videos from prior classes, for creating an effective video.

   It is critical that your video be short enough to remain engaging while delivering its content.
   Your video prototype should probably not be more than 2 minutes long.

   A modern phone can capture video of adequate quality for this assignment. 

3. Create a poster that communicates your design and your design process to a general audience.
   The goal is to present your work in a visual form to interested parties from across campus or from industry. 
   You need to quickly convey the most important aspects of your work. 
   The poster must be 32"x40" (portrait, vertical). 
   
4. Create a pitch that you can deliver together with your poster.
   This should summarize the problem and your design.
   It should be no more than 1 minute long.
   This pitch should convince the audience your problem was worth investigating and that your design effectively addresses it.

# Deliverables

<a name="initial_website"></a>

## 4a: Initial Website

Due: {{ page.due_project_4a }}

The goal of this milestone is to post an initial project website as part of the course website.

We will use your websites to advertise the poster session.
Although this is an initial website on which you will get feedback and will be able to update,
you should submit a complete and high-quality version of your website appropriate for advertising the course projects.

Your website will be served from a subdirectory of this course website.
It is also link via a thumbnail from the projects page:

[Projects Page]({{ site.baseurl }}/projects.html)

You can build your website however you like, but everything needed for your site must be in your directory.
Do not attempt to integrate with the Jekyll functionality used for this course website.
Simply build your website and submit the set of static files to be served from your directory. 

You will later add your video to the website. You may want to plan ahead for that additional content.

### Samples from Prior Offerings

Samples from prior offerings include:

{% for currentoffering in site.data.samples.offering %}{% for currentsample in site.data.samples[currentoffering.key] %}
  -  {{ currentoffering.name }} - [{{ currentsample.name }}]({{ currentsample.link }}){% endfor %}{% endfor %}
  
Note that details of assignments may have changed since prior offerings, so their reports may not map to the current project.
Also note these samples are intended to illustrate a variety of approaches, none of which is intended to be ideal or exemplary.
Be sure to understand and carefully consider project requirements and feedback from the course staff in the context of your own work.

### Submission

Submit a pull request containing your website. We will merge as quickly as possible. 
You can submit multiple requests as needed to fix issues or improve your website.
Your request should not modify anything outside your project website.

Submit simple pull requests early so that you become familiar with this functionality.
Do not wait until the final moments to begin to learn how to do this.

If you are absolutely unable to submit a pull request, submit via Canvas here:

{% if page.link_project_4a != nil %}<{{ page.link_project_4a }}>{% else %}`Link to be added`{% endif %}

### Grading

This milestone will be graded on a scale of __8 points__:

1.  __Completeness of Content__: (3 points)
2.  __Appropriately Polished Presentation__: (3 points)
3.  __Submitted via Pull Request__: (2 points)

Your website should be complete and will be evaluated as such.
But later critique and refinement will help further improve it before the final poster session.

<a name="initial_video_prototype"></a>

## 4b: Initial Video Prototype

Due: {{ page.due_project_4b }}

The goal of this milestone is to create a video that communicates your design to a broad audience.

Submit your video prototype in a portable and playable format.
It should be sufficiently high-resolution for projection, but sufficiently compressed that it can be played on a typical laptop. 
Specifically, it should be playable on a Windows laptop and Mac OS laptop without special codecs installed (e.g., H.264 in an mp4 container). 
It should be less than 50 MB in size. 

Remember it should probably not be more than 2 minutes long.

We have had good experiences encoding video using the open-source tool HandBrake together with its iPad preset.

If you contact us regarding early drafts of your video, we will test that they play properly.

### Samples from Prior Offerings

Samples from prior offerings include:

{% for currentoffering in site.data.samples.offering %}{% for currentsample in site.data.samples[currentoffering.key] %}
  -  {{ currentoffering.name }} - [{{ currentsample.name }}]({{ currentsample.link }}): [4b_{{ currentsample.suffix }}.mp4]({{ site.baseurl }}/samples/4b/4b_{{ currentsample.suffix }}.mp4){% endfor %}{% endfor %}

Note that details of assignments may have changed since prior offerings, so their reports may not map to the current project.
Also note these samples are intended to illustrate a variety of approaches, none of which is intended to be ideal or exemplary.
Be sure to understand and carefully consider project requirements and feedback from the course staff in the context of your own work.

### Submission

Submit via Canvas here: 

{% if page.link_project_4b != nil %}<{{ page.link_project_4b }}>{% else %}`Link to be added`{% endif %}

### Grading

This milestone will be graded on a scale of __6 points__:

1.  __Conveys Problem, Design, Context, and Satisfaction__: (3 points)
2.  __Appropriately Polished and Timed__: (3 points)

Your video prototype should be complete and will be evaluated as such.
But later critique and refinement will help further improve it before the final poster session.

<a name="poster_pitch"></a>

## 4c: Poster Critique and Pitch

Due: {{ page.due_project_4c }}

The goal of this milestone is to create a poster that communicates your design to a broad audience.

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

Be prepared to give your pitch.
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

{% if page.link_project_4c != nil %}<{{ page.link_project_4c }}>{% else %}`Link to be added`{% endif %}

Your poster may be in PPT, PPTX, or PDF format. 
We have a color plotter that can print posters this size. 
Your source file is due as above, we will then coordinate with you for proofreading and printing.

Be prepared to give your pitch.

### Grading

This milestone will be graded on a scale of __6 points__:

1.  __Initial Poster__: (3 points)
2.  __Initial Pitch__: (3 points)

<a name="communication_critique"></a>

## 4d: Communication Critique

Due: {{ page.due_project_4d }}

This is a flexible critique day. 
The purpose of this day is to help you refine whichever of your remaining deliverables you feel needs feedback. 
Be prepared to present your video, website, and/or poster. 
This is the last opportunity for you to get in-class critical feedback, so use it wisely.

### Submission

Bring at least one of your artifacts to class (e.g., be prepared to show them on a laptop).

<a name="final_everything"></a>

## 4e: Final Poster, Final Video, Final Website

Due: {{ page.due_project_4e }} 

Course staff need your finalized poster as soon as possible, to organize printing and preparing for the poster session.

Finalize your video prototype and website so we can finalize grading.

### Submission

Submit your final poster as soon as possible here:

Poster: {% if page.link_project_4e_poster != nil %}<{{ page.link_project_4e_poster }}>{% else %}`Link to be added`{% endif %}

Submit a pull request containing your website. We will merge as quickly as possible. 
You can submit multiple requests if needed to fix issues or improve your website.
Your request should not modify anything outside your project website.

Submit simple pull requests early so that you become familiar with this functionality.
Do not wait until the final moments to begin to learn how to do this.

Depending on how you embed your video in your website, it may or may not be part of the pull request.
For example, embedding a YouTube or Vimeo player does not give us your video.
We therefore explicitly ask that final videos also be submitted via Canvas here: 

Video: {% if page.link_project_4e_video != nil %}<{{ page.link_project_4e_video }}>{% else %}`Link to be added`{% endif %}

### Grading

Your final video, final website, and final poster will each be graded on a scale of __10 points__.

#### Poster

- __Content__: (5 points)
  - Includes all of the points listed above
  - Key features of the design are clear
  - Gives insight into the design process
- __Presentation__: (5 points)
  - Large images that show the key parts of the design
  - Only minimal and appropriate use of text
  - Text is large and legible
  - Colors and fonts are a pleasing combination and easy to read

#### Video Prototype

- __Content__: (7 points)
  - Conveys the problem addressed by the design
  - Conveys the design itself
  - Conveys the context of interaction
  - Conveys the satisfaction of the design  
- __Presentation__: (3 points)
  - Reasonable level of production value
  - Appropriately edited and paced

#### Website

- __Content__: (5 points)
  - Includes all of the points listed above
  - Key features of the design are clear
  - Gives insight into the design process
  - Links to your reports and video prototype
- __Presentation__: (5 points)
  - Looks professional and is something you would consider including in a design portfolio

<a name="team_peer_feedback"></a>

## 4f: Team Peer Feedback

Due: {{ page.due_project_4f }}

Submit peer feedback using the form distributed to the class by email.

<a name="poster_session"></a>

## 4g: Poster Session

Attend {{ page.due_project_4g }}.

Come to the poster session to show off your work and engage with your classmates.
Present your pitch to a team of judges.

Take the opportunity present your work, chat with judges,
engage with other students, and reflect on a busy and productive quarter.

We will not be conducting any evaluation at the poster session itself. 
