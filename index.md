---
---

# Blogs

Here are my blogs

{% for post in site.posts %}
* [{{ post.title }}]({{ post.url }})
{% endfor %}
