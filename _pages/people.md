---
title: "People"
layout: splash
permalink: /people
author_profile: false
---


<h2>{{ page.title }}</h2>

{% assign authors = site.data.authors | sort %}

<div class="grid__wrapper">

{% for f in authors %}
  {% assign author = f[1] %}
    {% if author.status == "employee" %}
      {% include profile-single.html type="grid" author=author %}
    {% endif %}
{% endfor %}
</div>

<div style="clear: both;"></div>
<h3>PhD Students</h3>
<div class="grid__wrapper">

{% for f in authors %}
  {% assign author = f[1] %}
    {% if author.status == "phdstudent" %}
      {% include profile-single.html type="grid" author=author %}
    {% endif %}
{% endfor %}
</div>

<div style="clear: both;"></div>
<h3>Collaborators</h3>
<div class="grid__wrapper">

{% for f in authors %}
  {% assign author = f[1] %}
    {% if author.status == "collaborator" %}
      {% include profile-single.html type="grid" author=author %}
    {% endif %}
{% endfor %}
</div>
