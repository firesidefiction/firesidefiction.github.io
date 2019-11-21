---
layout: default
title: Fireside Contributors
permalink: /contributors
---

<h1>Contributors</h1>

<h1>Editors</h1>
<ul>
  {% for contributor in site.contributors %}
  {% if contributor.role == "editor" or contributor.role-2 == "editor" %}
    <li>
      <h2><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></h2>
      <h3>{{ contributor.title }}</h3>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h1>Authors</h1>
<ul>
  {% for contributor in site.contributors %}
  {% if contributor.role == "author" %}
    <li>
      <h2><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></h2>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h1>Illustrators</h1>
<ul>
  {% for contributor in site.contributors %}
  {% if contributor.role == "illustrator" %}
    <li>
      <h2><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></h2>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h1>Narrators</h1>
<ul>
  {% for contributor in site.contributors %}
  {% if contributor.role == "narrator" %}
    <li>
      <h2><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></h2>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h1>Translators</h1>
<ul>
  {% for contributor in site.contributors %}
  {% if contributor.role == "translator" %}
    <li>
      <h2><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></h2>
    </li>
    {% endif %}
  {% endfor %}
</ul>
