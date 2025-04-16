---
title: Sample Letter Archive
layout: base.njk
---

<h1>Historical Letter Archive</h1>
<p>Welcome to the collection. Use the tags below to explore letters by category.</p>

<ul class="tags">
  {% for tag in collections.tagList %}
    <li><a href="/tags/{{ tag | slug }}">{{ tag }}</a></li>
  {% endfor %}
</ul>

<div class="grid">
  {% for letter in collections.letters | reverse %}
    <div class="card">
      <a href="{{ letter.url }}">
        <img src="{{ letter.data.image }}" alt="{{ letter.data.title }}" />
        <h2>{{ letter.data.title }}</h2>
        <p>{{ letter.data.date }}</p>
      </a>
    </div>
  {% endfor %}
</div>
