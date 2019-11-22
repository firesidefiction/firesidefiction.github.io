---
layout: default
title: Fireside Contributors
permalink: /contributors
---

<h1>Contributors</h1>

<h2>Editors</h2>
<ul>
  {% for contributor in site.contributors %}
  {% if contributor.role == "editor" or contributor.role-2 == "editor" %}
    <li>
      <p><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a> | {{ contributor.title | markdownify }}</p>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h2>Authors</h2>
<ul>
  {% for contributor in site.contributors %}
  {% if contributor.role == "author" %}
    <li>
      <p><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></p>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h2>Illustrators</h2>
<ul>
  {% for contributor in site.contributors %}
  {% if contributor.role == "illustrator" %}
    <li>
      <p><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></p>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h2>Letterers</h2>
<ul>
  {% for contributor in site.contributors %}
  {% if contributor.role == "letterer" %}
    <li>
      <p><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></p>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h2>Narrators</h2>
<ul>
  {% for contributor in site.contributors %}
  {% if contributor.role == "narrator" %}
    <li>
      <p><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></p>
    </li>
    {% endif %}
  {% endfor %}
</ul>

<h2>Translators</h2>
<ul>
  {% for contributor in site.contributors %}
  {% if contributor.role == "translator" %}
    <li>
      <p><a href="{{ contributor.url }}">{{ contributor.credit-name }}</a></p>
    </li>
    {% endif %}
  {% endfor %}
</ul>
