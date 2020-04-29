---
---

# Blogs

Here are my blogs

{% for post in site.posts %}
* [{{ post.title }}]({{site.baseurl}}{{ post.url }})
{% endfor %}
