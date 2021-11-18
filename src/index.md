---
title: Hello Vinh
layout: "base.njk"
---

Hello Jamstack !

<!-- {% for post in collections.posts %}
- [{{ post.data.title }}]({{ post.url }})
{% endfor %} -->

<ul>
{% for post in collections.posts %}
<li><a href="{{ post.url }}">{{ post.data.title }}</a></li>
{% endfor %}
</ul>

{% image "./src/images/the-lucky-neko.jpg", "photo of my cat" "(min-width: 200px) 500px, 800px, 1100px" %}
