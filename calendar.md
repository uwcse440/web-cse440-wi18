---
layout: base/bar/bar-sidebar-none
title: Calendar
---

{% comment %} Starting from the first date of instruction, find Sunday {% endcomment %}
{% assign startdateseconds = site.data.calendar.dates_of_instruction.start | append: 'Z' | date: '%s' %}
{% assign startdate = startdateseconds | date: '%F' %}

{% comment %} Starting from the last date of instruction, find Saturday {% endcomment %}
{% assign enddateseconds = site.data.calendar.dates_of_instruction.end | append: 'Z' | date: '%s' %}
{% assign enddate = enddateseconds | date: '%F' %}

{% comment %} How many days are in our calendar, adding 3600s in case of DST change {% endcomment %}
{% assign numdays = enddateseconds | minus: startdateseconds | plus: 3600 | divided_by: 86400 %}

<div class="calendar">

<!--div class="row week">
<div class="col-xs-12">
<div class="alert alert-danger" markdown="1">
This page is still being migrated and developed. All content remains subject to change.
</div>
</div>
</div-->

  {% for currentdaynum in (0..numdays) %}
    {% assign currentdateseconds = currentdaynum | times: 86400 | plus: 3600 | plus: startdateseconds %}
    {% assign currentdate = currentdateseconds | date: '%F' %}
    {% assign currentdayofweek = currentdate | date: '%a' %}

    {% case currentdayofweek %}
    {% when 'Sun' %}
    <div class="row week">
    {% when 'Mon' or 'Tue' or 'Wed' or 'Thu' or 'Fri' %}
    <div class="col-md-2-4 day">
      {{ currentdate | date: '%b %-d'}}<br>

        {% for currentholiday in site.data.calendar.holidays %}
          {% if currentdate == currentholiday.date %}
            <div class="item holiday">
              {{ currentholiday.name }}
            </div>
          {% endif %}
        {% endfor %}

        {% for currentaway in site.data.calendar.aways %}
          {% if currentdate == currentaway.date %}
            <div class="item away">
              {{ currentaway.name }}
            </div>
          {% endif %}
        {% endfor %}

        {% for currentlecture in site.data.calendar.lectures %}
          {% if currentdate == currentlecture.date %}
            {% assign currentlocation = currentlecture.location %}
            {% if currentlocation == nil %}
              {% assign currentlocation = "lectures" %}
            {% endif %}

            <div class="item lecture">
              {% if currentlecture.name != nil %}
                {{ currentlecture.name }}
              {% else %}
                Lecture
              {% endif %}
              <br>
              {% if currentlecture.slides != nil %}
                [<a href="{{ site.baseurl }}/{{ currentlecture.slides }}">slides</a>]
              {% endif %}
              {% if currentlecture.panopto != nil %}
                [<a href="{{ currentlecture.panopto }}">video</a>]
              {% endif %}
              {% if currentlecture.slides != nil or currentlecture.video != nil %}
                <br>
              {% endif %}
              <small>
                {% for currentlocationitem in site.data.calendar.locations[currentlocation] %}
                    {{ currentlocationitem.time }} |
                    {{ currentlocationitem.location }}<br>
                {% endfor %}
              </small>
            </div>
          {% endif %}
        {% endfor %}

        {% for currentsection in site.data.calendar.sections %}
          {% if currentdate == currentsection.date %}
            {% assign currentlocation = currentsection.location %}
            {% if currentlocation == nil %}
              {% assign currentlocation = "sections" %}
            {% endif %}

            <div class="item section">
              {% if currentsection.slides != nil %}
                <a href="{{ site.baseurl }}/{{ currentsection.slides }}">
              {% endif %}
                {% if currentsection.name != nil %}
                  {{ currentsection.name }}<br>
                {% else %}
                  Section<br>
                {% endif %}
              {% if currentsection.slides != nil %}
                </a>
              {% endif %}
              <small>
                {% for currentlocationitem in site.data.calendar.locations[currentlocation] %}
                    {{ currentlocationitem.time }} |
                    {{ currentlocationitem.location }}<br>
                {% endfor %}
              </small>
            </div>
          {% endif %}
        {% endfor %}

        {% for currentmajor in site.data.calendar.majors %}
          {% if currentdate == currentmajor.date %}
            {% assign currentlocation = currentmajor.location %}
            <div class="item major">
              {% if currentmajor.link != nil %}<a href="{{ site.baseurl }}/{{ currentmajor.link }}">{% endif %}
                {{ currentmajor.name }}<br>
                {% if currentmajor.link != nil %}</a>{% endif %}
              <small>
                {% for currentlocationitem in site.data.calendar.locations[currentlocation] %}
                    {{ currentlocationitem.time }} |
                    {{ currentlocationitem.location }}<br>
                {% endfor %}
              </small>
            </div>
          {% endif %}
        {% endfor %}

        {% for currentassignment in site.data.calendar.assignments %}
          {% if currentdate == currentassignment.date %}
            <div class="item assignment">
              <small>
                  {% if currentassignment.link != nil %}<a href="{{ site.baseurl }}/{{ currentassignment.link }}">{% endif %}
                  {{ currentassignment.name }}<br>
                  {% if currentassignment.duenote != nil %}{{ currentassignment.duenote }}{% endif %}
                  {% if currentassignment.link != nil %}</a>{% endif %}
              </small>
            </div>
          {% endif %}
        {% endfor %}

        {% for currentofficehour in site.data.calendar.officehours %}
          {% if currentdate == currentofficehour.date %}
            {% assign currentlocation = currentofficehour.location %}
            <div class="item officehour">
              <small>
                {{ currentofficehour.name }}<br>
                {% for currentlocationitem in site.data.calendar.locations[currentlocation] %}
                  {{ currentlocationitem.time }}<br>
                  {{ currentlocationitem.location }}<br>
                {% endfor %}
              </small>
            </div>
          {% endif %}
        {% endfor %}
    </div>
    {% when 'Sat' %}
    </div>
    {% endcase %}
  {% endfor %}
</div>
