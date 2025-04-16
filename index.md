---
title: The Book – A Letter & Signature Archive
layout: base.njk
---

<h1>The Book</h1>

<p><em>The Book</em> is a collection of letters and autographs compiled by C. W. Mills in the early 1890s. It captures the voices of presidents, generals, authors, reformers, and cultural figures from late 19th-century America.</p>

<hr>

<h2>Highlighted Letters</h2>
<div class="featured-grid">
  <div class="card">
    <a href="/letters/frances-willard/">
      <img src="/images/letters/Frances_Willard_Letter.jpg" alt="Frances Willard">
      <h3>Frances Willard</h3>
      <p>“Tell me with whom thou goest...”</p>
    </a>
  </div>
  <div class="card">
    <a href="/letters/john-russell-young/">
      <img src="/images/letters/John_Russell_Young_Letter.jpg" alt="John Russell Young">
      <h3>John Russell Young</h3>
      <p>Union League, Philadelphia – 1894</p>
    </a>
  </div>
</div>

<hr>

<h2>Explore by Category</h2>
<div class="category-nav">
  <a href="/tags/military/">Military & Government</a>
  <a href="/tags/authors/">Authors & Poets</a>
  <a href="/tags/reformers/">Activists & Reformers</a>
  <a href="/tags/religious/">Religious Figures</a>
  <a href="/tags/later-collection/">Later Acquisitions</a>
  <a href="/tags/signatures/">Signature Collections</a>
</div>

<hr>

<h2>Recent Additions</h2>
<ul>
  {% for letter in collections.letters | reverse | limit(6) %}
    <li><a href="{{ letter.url }}">{{ letter.data.title }}</a> ({{ letter.data.date }})</li>
  {% endfor %}
</ul>

<style>
.featured-grid {
  display: flex;
  gap: 1rem;
  margin-bottom: 2rem;
  flex-wrap: wrap;
}
.featured-grid .card {
  width: 250px;
  border: 1px solid #ccc;
  border-radius: 8px;
  overflow: hidden;
  background: #fff;
  padding: 0.5rem;
  text-align: center;
}
.featured-grid img {
  width: 100%;
  height: auto;
  margin-bottom: 0.5rem;
}
.category-nav {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  margin: 1rem 0;
}
.category-nav a {
  background: #eee;
  padding: 0.5rem 1rem;
  border-radius: 5px;
  text-decoration: none;
  color: #333;
  font-weight: bold;
}
</style>
