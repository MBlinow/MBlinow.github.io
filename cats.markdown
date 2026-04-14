---
layout: archive
title: "Cats"
permalink: /cats/
---

{% assign cat_posts = site.posts | where_exp: "post", "post.categories contains 'cats'" %}
{% if cat_posts.size > 0 %}
  {% for post in cat_posts %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
  <p>No cat posts yet — check back soon!</p>
{% endif %}
