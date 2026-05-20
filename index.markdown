---
layout: archive
title: "Matt Blinow"
---

## Cats

{% assign cat_posts = site.posts | where_exp: "post", "post.categories contains 'cats'" %}
{% if cat_posts.size > 0 %}
  {% for post in cat_posts limit:3 %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
  <p>No cat posts yet — check back soon!</p>
{% endif %}

---

<!-- Future sections go here, e.g.:

## Life
{% assign life_posts = site.posts | where_exp: "post", "post.categories contains 'life'" %}
...

-->
