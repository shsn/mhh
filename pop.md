---
layout: default
title: Pop Artists
---

<h1>Pop Artists</h1>

<ul>
{% for artist in site.data.artists %}
  <li>
    <a href="{{ artist.url | relative_url }}">
      <img src="{{ artist.image }}" alt="{{ artist.name }}">
      <h2>{{ artist.name }}</h2>
      <p>{{ artist.description }}</p>
    </a>
  </li>
{% endfor %}
</ul>