---
layout: default
id: home
title: CSE 201 Schedule
---

- hi
- [Assignment 1](assignments/Assignment1.pdf)
- [Assignment 2](assignments/Assignment2.pdf)
- [Assignment 3](assignments/Assignment3.pdf)
- [Assignment 4](assignments/Assignment4.pdf)

<ul>
  {% for post in site.posts %}
    <li>
      <a href="./{{ post.id }}.html">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>


<div>
  {% for page in site.pages %}
    {% if page.id != 'home' %} 
      <div>Deadline: {{ page.deadline }}</div>
      <div>ID: {{ page.id }}</div>
      <div>Points: {{ page.points }}</div>
      <div>Deliverable: <a href="./{{ page.id }}.html">{{ page.title }}</a></div>
      <div>Notes: {{ page.notes }}</div>
    {% endif %}
  {% endfor %}
</div>

<div>
  {% for page in site.pages %}
    {% if page.id != 'home' %} 
      <div>Deadline: {{ page.deadline }}</div>
      <div>ID: {{ page.id }}</div>
      <div>Points: {{ page.points }}</div>
      <div>Deliverable: <a href=".{{ page.url }}">{{ page.title }}</a></div>
      <div>Notes: {{ page.notes }}</div>
    {% endif %}
  {% endfor %}
</div>


