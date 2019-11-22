---
layout: default
title: Fireside Contributors
permalink: /contributors
---

<h1>Contributors</h1>

<h2>Editors</h2>
<ul class="multicol">
  {% assign editors = site.contributors | sort: 'last-name' %}
  {% for contributor in editors %}
  {% if contributor.role == "editor" or contributor.role-2 == "editor" or contributor.role-3 == "editor" %}
    <li>
      <a href="{{ contributor.url }}">{{ contributor.credit-name }}</a><small>{{ contributor.title | markdownify }}</small>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h2>Authors</h2>
<ul class="multicol">
    {% assign authors = site.contributors | sort: 'last-name' %}
    {% for contributor in authors %}
      {% if contributor.role == "author" %}
        <li><p><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></p></li>
      {% endif %}
    {% endfor %}
</ul>

<h2>Illustrators</h2>
<ul class="multicol">
  {% assign illustrators = site.contributors | sort: 'last-name' %}
  {% for contributor in illustrators %}
  {% if contributor.role == "illustrator" %}
    <li>
      <p><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></p>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h2>Letterers</h2>
<ul class="multicol">
  {% assign letterers = site.contributors | sort: 'last-name' %}
  {% for contributor in letterers %}
  {% if contributor.role == "letterer" %}
    <li>
      <p><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></p>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h2>Narrators</h2>
<ul class="multicol">
  {% assign narrators = site.contributors | sort: 'last-name' %}
  {% for contributor in narrators %}
  {% if contributor.role == "narrator" %}
    <li>
      <p><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></p>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h2>Translators</h2>
<ul class="multicol">
  {% assign translators = site.contributors | sort: 'last-name' %}
  {% for contributor in translators %}
  {% if contributor.role == "translator" %}
    <li>
      <p><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></p>
    </li>
    {% endif %}
  {% endfor %}
</ul>
