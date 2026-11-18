---
layout: single
title: "Personal"
permalink: /personal/
author_profile: true
classes: wide
---

In a past life, I wanted to be a journalist. Here are some articles I wrote:

<div class="personal-articles">
  {% for article in site.data.personal_articles %}
  <article class="personal-article">
    <a class="personal-article__link" href="{{ article.url | escape }}">
      <img class="personal-article__thumbnail" src="{{ article.image | relative_url }}" alt="{{ article.image_alt | escape }}" width="640" height="400" loading="lazy" decoding="async">
      <div class="personal-article__body">
        <p class="personal-article__publication">{{ article.publication | escape }}{% if article.date %} · <time datetime="{{ article.date | date: '%Y-%m-%d' }}">{{ article.date | date: '%B %-d, %Y' }}</time>{% endif %}</p>
        <h2>{{ article.title | escape }}</h2>
        <span class="personal-article__read">Read article <span aria-hidden="true">↗</span></span>
      </div>
    </a>
  </article>
  {% endfor %}
</div>

You can also browse my [BusinessLine author page](https://www.thehindubusinessline.com/profile/author/Kavya-Ravindranath/).
