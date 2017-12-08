---
layout: base/bar/bar-sidebar-none
title: Course Overview
---

<div class="alert alert-danger" markdown="1">
This page is still being migrated and developed. All content remains subject to change.
</div>

# Course Description

This course provides an introduction to human-computer interaction and the design process.
Students will learn methods and skills for designing and prototyping interactive systems.
The course covers a design process from the initial formulation of a design problem to creation of digital prototypes.
The course structure is a mix of lectures, classroom activities, and design critiques by peers and course staff.
The course is overwhelmingly organized around a group project, in which students:

- Ideate and Propose Design Problems
- Study Existing Practices and Challenges
- Explore Potential Design Opportunities and Tradeoffs
- Evaluate and Improve a Design
- Communicate their Problem and Resulting Design

## Learning Objectives

- Process-Focused Perspective on Interaction Design
- Design Research Methods and Skills
- Task-Focused Scenario Development, Sketching, and Storyboarding
- Rapid Prototyping and Iteration
- Critical Perspective on Design Solutions

# Course Staff

<html>
  <div class="row">
    <div class="col-md-2">
      <p>James Fogarty</p>
      <p><img src="{{ site.baseurl }}/images/james_photo.jpg" height="140" alt="James Fogarty"/></p>
    </div>
    <div class="col-md-2">
      <p>Kailey Chan</p>
      <p><img src="{{ site.baseurl }}/images/kailey_photo.png" height="140" alt="Kailey Chan"/></p>
    </div>
    <div class="col-md-2">
      <p>Dhruv Jain</p>
      <p><img src="{{ site.baseurl }}/images/dhruv_photo.jpg" height="140" alt="Dhruv Jain"/></p>
    </div>
    <div class="col-md-2">
      <p>Nigini Oliveira</p>
      <p><img src="{{ site.baseurl }}/images/nigini_photo.jpg" height="140" alt="Nigini Oliveira"/></p>
    </div>
    <div class="col-md-2">
      <p>Chris Seeds</p>
      <p><img src="{{ site.baseurl }}/images/chris_photo.jpg" height="140" alt="Chris Seeds"/></p>
    </div>
    <div class="col-md-2">
      <p>Jihoon Suh</p>
      <p><img src="{{ site.baseurl }}/images/jihoon_photo.jpg" height="140" alt="Jihoon Suh"/></p>
    </div>
  </div>
</html>

# Basic Information

__Contact__:

- Email all instructors at cse440-staff [at] cs.washington.edu

__Class Time & Location__:

- Tuesdays & Thursdays, 12:00-1:20 [PAA A110](http://www.washington.edu/students/maps/map.cgi?PAA)

Check the calendar for non-standard times or locations. 

__Section Times & Locations__: 

- Fridays, 9:30-10:20 [MGH 058](http://www.washington.edu/students/maps/map.cgi?MGH), with Nigini, Dhruv, Chris
- Fridays, 10:30-11:20 [MGH 058](http://www.washington.edu/students/maps/map.cgi?MGH), with Nigini, Dhruv, Chris
- Fridays, 12:30-1:20 [MGH 058](http://www.washington.edu/students/maps/map.cgi?MGH), with Kailey, Dhruv, Jihoon
- Fridays, 1:30-2:20 [MGH 058](http://www.washington.edu/students/maps/map.cgi?MGH), with Kailey, Dhruv, Jihoon

Check the calendar for non-standard times, locations, or staffing. 

__Office Hours__: 

- James, Tuesdays 3:30 to 4:30, CSE 632
- Kailey, Wednesdays, 3:30 to 4:30, CSE 021
- Dhruv, Thursdays, 1:30 to 2:30, CSE 021
- Nigini, Mondays, 3:30 to 4:30, CSE 021

Scheduled hours are held most weeks, but check the calendar. Other meetings are by appointment.

# Project Theme

People have long sought to better understand themselves, but technology advances enable new approaches.
Students will examine problems people encounter in gathering and gaining value from personal data,
then explore how new technology can go beyond simple data fetishes to help people in using personal data as part of reaching their goals.

Understanding and designing for self-tracking is also known as personal informatics:

> Personal informatics systems are systems that help people collect personally relevant information for the purpose of 
> self-reflection and gaining self-knowledge.
>
> [Li _et al._, 2010]({{ site.baseurl }}/readings/PersonalInformatics-Li2010.pdf).

Self-tracking and personal informatics are related to the [Quantified Self](http://quantifiedself.com/) movement, which describes itself as:

> Self-knowledge through numbers.
>
> [Gary Wolf, 2009](http://archive.wired.com/medtech/health/magazine/17-07/lbnp_knowthyself)

As a focus for Autumn 2017, we will ask students to explore __tracking beyond the self__.
Instead of limiting self-tracking to dashboards for an isolated self-analyst,
we will ask students to consider the many different ways people might gather and interact around personal data.

Tracking can therefore take many mobile forms:

- wearable sensors
- phone and watch applications
- appliances and other artifacts in the environment
- hybrid forms (e.g., semi-automated capture, mobile capture with later annotation or review)

Tracking can include many social contexts:

- co-located relationships (e.g., families, friends, co-workers)
- remote relationships (e.g., families, friends, co-workers)
- communities organizing (e.g., people in a building, community volunteers)
- people seeking help from peers (e.g., social sharing, support networks)
- people seeking help from experts (e.g., health providers)

And tracking can explore new forms of interaction:

- conversational interfaces
- tangible interfaces
- ubiquitous computing interfaces (e.g., enabled by the Internet of Things) 

Any problem where people gather or seek value in personal data
introduces opportunities and challenges in designing for effective interaction around that data.

# Project Structure

Projects are organized around four assignments, each consisting of several milestones:

- [Assignment 1 - Project Proposal]({{ site.baseurl }}/assignments/assignment1/)
- [Assignment 2 - Getting the Right Design]({{ site.baseurl }}/assignments/assignment2/)
- [Assignment 3 - Getting the Design Right]({{ site.baseurl }}/assignments/assignment3/)
- [Assignment 4 - Communicating the Design]({{ site.baseurl }}/assignments/assignment4/)

Sample projects from prior offerings include:

{% for currentoffering in site.data.samples.offering %}{% for currentsample in site.data.samples[currentoffering.key] %}
  -  {{ currentoffering.name }} - [{{ currentsample.name }}]({{ currentsample.link }}){% endfor %}{% endfor %}

Note that details of assignments may have changed since prior offerings, so their reports may not map to the current project.
Also note these samples are intended to illustrate a variety of approaches, none of which is intended to be ideal or exemplary.
Be sure to understand and carefully consider project requirements and feedback from the course staff in the context of your own work.

# Readings

A small set of readings are assigned throughout the quarter, with additional resources also made available.

- [Reading Assignments]({{ site.baseurl }}/assignments/readings/)

# Grading

Strive to do good work because you care about your own opportunities to learn,
including the opportunities this course provides in working with a group in an intensive project.

The overall course grade will be computed as follows:

- Group Project (__65%__)
  - Assignment 1, Project Proposal (__3%__)
  - Assignment 2, Getting the Right Design (__21%__)
    - Milestones (__6%__)
    - Final Report (__15%__)
  - Assignment 3, Getting the Design Right (__14%__)
    - Milestones (__4%__)
    - Final Report (__10%__)
  - Assignment 4, Communicating the Design (__15%__)
    - Milestones (__3%__)
    - Project Website (__4%__)
    - Video Prototype (__4%__)
    - Poster (__4%__)
  - Presentations (__12%__)
    - Getting the Right Design Presentation (__5%__)
    - Getting the Design Right Presentation (__5%__)
    - Individual Presentation Score (__2%__)
- Exam (__25%__)
- Individual Readings (__5%__)
- Participation (__5%__)

Each assignment will also provide a point breakdown intended to convey how it will be graded. 
Design is an inherently subjective practice, and so grading in this course is necessarily subjective.
The stated project requirements are the minimum, leaving room for groups to wow us with your work.

Because the course is designed around feedback on project milestones, grades given to those milestones indicate
that you have invested sufficient effort and insight at the time of the milestone.
You will get feedback and are expected to continue acting upon that feedback in your design process.
The bulk of project grades is therefore attached to the final deliverables, which are evaluated on their quality.

We expect groups to take collective responsibility and to resolve any coordination issues.
The course staff is always happy to make suggestions with regard to your effort and coordination.
If an issue needs to be raised with the course staff, we expect it to be raised early enough to be addressed.
If necessary, we reserve the ability to adjust an individual's grade with regard to the group project.

<a name="submission"></a>

# Submission

Many assignments are due "the night before class". We will implement this in Canvas as 11:59pm.
In order to be prepared to give you feedback, the course staff must have your submission in the morning.
Submitting the day of class, just before class, or in class is therefore unacceptable, risking zero credit.

Submissions should be in PDF format (i.e., not plain text, not Word). 
The PDF should be printable, containing everything we need to review and grade the assignment (e.g., your name).
The course staff has a large number of submissions to manage, so format and completeness issues are problematic.

<a name="projects"></a>

# Contributing

This course website lives on GitHub:

<https://github.com/uwcse440/web-cse440-au17>

You can submit pull requests to update the webpage, and you will publish project webpages via pull request.

