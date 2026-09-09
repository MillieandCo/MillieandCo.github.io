---
layout: single
title: false
permalink: /
author_profile: false
---

<div style="background-color: #F79494; border-radius: 24px; padding: 4rem 2rem; text-align: center; color: white; margin-bottom: 3rem;">
  <h1 style="font-size: 2.75rem; font-weight: 800; margin-bottom: 0.75rem;">Spoil Your Cat 🐾</h1>
  <p style="font-size: 1.15rem; max-width: 550px; margin: 0 auto 1.5rem;">
    Curated products, honest reviews, and real cat-care advice — inspired by our own Millie.
  </p>
  <a href="/products/" style="display: inline-block; background: white; color: #E67979; font-weight: 700; text-transform: uppercase; letter-spacing: 0.05em; padding: 0.85rem 2rem; border-radius: 30px; text-decoration: none;">Shop Millie's Picks</a>
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

<div style="background: white; border-radius: 20px; padding: 2.5rem; margin-top: 3rem; text-align: center; box-shadow: 0 4px 14px rgba(0,0,0,0.05);">
  <h2 style="margin-bottom: 1.5rem;">What Cat Parents Are Saying</h2>
  <p style="color: #F2C14E; font-size: 1.5rem; margin-bottom: 0.5rem;">★★★★★</p>
  <p style="font-style: italic; max-width: 500px; margin: 0 auto;">
    "Millie's recommendations actually helped — my cat loves the scratching post and I love that the reviews were honest, not just copied specs."
  </p>
</div>
