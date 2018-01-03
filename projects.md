---
layout: base/bar/bar-sidebar-right
title: Projects
---

<div class="sidebar_start"></div>

<div class="row">
<div class="col-md-12" markdown="block">
<div class="panel panel-default" style="margin-top:20px;">
<div class="panel-heading" markdown="block">
## Poster Session
</div>
<div class="panel-body" markdown="block">
Please join us for a poster session celebrating the outstanding design work of CSE 440 students:
{% comment %}
Thank you for joining us to celebrate the outstanding design work of CSE 440 students:
{% endcomment %}

Tuesday, June 6

11:00 am to 11:50pm, [CSE Atrium](http://www.washington.edu/maps/#!/cse)

<img src="{{ site.baseurl }}/images/poster_session.jpg" width="100%" alt="Poster Session"/>
</div>
</div>
</div>
</div>

<div class="sidebar_end"></div>

<div class="alert alert-danger" markdown="1">
This page is still being migrated and developed.
Information here is likely suggestive of the final page, but remains subject to change.
Test build text inserted by James.
</div>

# Project Theme


This year’s project theme will be “Designing for diversity”! You will be encouraged to design for groups of people who are different from yourself and/or to design for inclusiveness, connecting people from different backgrounds. 

Computers and the Internet have changed many people's lives. However, many applications that we use in our daily lives are developed by Westerners and embed the developers' beliefs in what is useful and usable. 
For example, Facebook is extremely popular in many Western countries, but has failed to attract a large user base in Russia. Facebook is also not as popular with elderly and teens as it is with people between 25 and 45 of age. Similarly, Uber and Lyft have gained much attraction with economically prosperous young professionals, but are often seen with suspicion in economically strained parts of the US. Most of these problems in designing adequate technology and gaining market share arise because designers and developers can be insufficiently aware of the beliefs, preferences, needs, and prior experiences of people who are different from themselves.

Over the course of the quarter, you will work as a group on designing a system to an activity or relationship within the particular context of a group of people that is not particularly well supported by current tools. Example groups that you could design for are: 
- Minorities 
- Homeless
- People with disabilities
- People from different cultures
- People with chronic conditions
- Elderly
- Local business owners
- Workers
- Interactions between these groups (or between yourselves and one of these groups)

As part of your project, you will need to define what a specific group's needs are that your project tries to support and what activity you would like to design that might help address this need.
Think about how that activity is currently supported via technology, what doesn't work about current ways of supporting it, and how your solution will do this better. 
The specificity of addressing a particular group of people allows you to deeply think about what makes the group unique and how you would best want to support them. So, dive in and see what you can come up with! 

# Project Websites

{% assign projects_count = site.data.projects.projects | size %}
{% assign projects_rows = projects_count | divided_by: 4 | plus: 1 %}

{% if projects_count == 0 %}
Will be linked here as course projects are proposed and developed.
{% endif %}

<div class="row">
  {% for item_project in site.data.projects.projects %}
    <div class="col-sm-3 col-xs-6">        
      <p>
        {% if item_project.publishlink %}
        <a href="{{ site.baseurl }}/projects/{{ item_project.path }}/" target="_blank">
          {{ item_project.name }}
        </a>
        {% else %}
          {{ item_project.name }}
        {% endif %}
      </p>
      <div class="thumbnailBox">
        {% if item_project.publishlink %}
        <a href="{{ site.baseurl }}/projects/{{ item_project.path }}/" target="_blank">
          <img src="{{ site.baseurl }}/projects/{{ item_project.path }}/project_thumb.png" width="150" class="projectThumbnail" alt="{{ item_project.name }}"/>
        </a>
        {% else %}
          <img src="{{ site.baseurl }}/projects/{{ item_project.path }}/project_thumb.png" width="150" class="projectThumbnail" alt="{{ item_project.name }}"/>
        {% endif %}
      </div>
      {% assign row_current = forloop.index | minus: 1 | divided_by: 4 | plus: 1 %}
      {% unless row_current == projects_rows %}
        <p>&nbsp;</p>
      {% endunless %}
    </div>
  {% endfor %}
</div>