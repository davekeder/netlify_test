---
title: Letter from Frances Willard
date: 1893-11-07
layout: base.njk
tags: [reformers, women's rights]
image: ../images/letters/Frances_Willard_Letter.jpg
permalink: /letters/frances-willard/
---


<div class="letter-header">
  <h1>{{ title }}</h1>
  <p><strong>Date:</strong> {{ date }}</p>
  <p><strong>Tags:</strong> {% for tag in tags %}<a href="/tags/{{ tag | slug }}">{{ tag }}</a>{% if not loop.last %}, {% endif %}{% endfor %}</p>
</div>

<div class="letter-body">
  <div class="letter-image">
    <img src="{{ image }}" alt="Letter from Frances Willard">
  </div>

  <div class="letter-transcription">
    <h2>Transcription</h2>
    <blockquote>
      <p>Dear Friend,</p>
      <p>You are kind to enquire as to when I expect to return to America; the year that Doctor Benjamin Ward Richardson said I must have will end in June next, and I really hope to go home by that time.</p>
      <p>I am much interested to know of your relationship with a leader in the cause to which I am devoted, and I hope that you, his son, will prove to be a worthy successor. Remember the priceless motto "Tell me with whom thou goest, and I will tell thee what thou doest."</p>
      <p>Believe me, ever your sincere friend,</p>
      <p><strong>Frances Willard</strong></p>
    </blockquote>
  </div>
</div>
