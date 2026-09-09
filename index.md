---
layout: single
title: false
permalink: /
author_profile: false
---

<div style="background: linear-gradient(135deg, #FF6F61, #FFC857); border-radius: 20px; padding: 3rem 2rem; text-align: center; color: white; margin-bottom: 2.5rem;">
  <h1 style="font-size: 2.5rem; margin-bottom: 0.5rem;">Millie & Co. 🐾</h1>
  <p style="font-size: 1.2rem; max-width: 600px; margin: 0 auto;">
    Real cat care advice, honest product picks, and a whole lot of Millie.
  </p>
</div>

## 🐱 Latest Care Guides

<div class="feature__wrapper">
  {% assign guides = site.care_guides | sort: 'date' | reverse | slice: 0, 3 %}
  {% for guide in guides %}
    <div class="feature__item">
      <div class="archive__item">
        <h3><a href="{{ guide.url }}">{{ guide.title }}</a></h3>
        <p>{{ guide.excerpt }}</p>
      </div>
    </div>
  {% endfor %}
</div>

## 🛒 Top-Rated Products

<div class="feature__wrapper">
  {% assign items = site.products | sort: 'date' | reverse | slice: 0, 3 %}
  {% for item in items %}
    <div class="feature__item">
      <div class="archive__item">
        <h3><a href="{{ item.url }}">{{ item.title }}</a></h3>
        <p>{{ item.excerpt }}</p>
      </div>
    </div>
  {% endfor %}
</div>
