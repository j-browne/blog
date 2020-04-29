---
---

# Blogs

Here are my blogs

{% for post in site.posts reversed %}
* [{{ post.title }}]({{site.baseurl}}{{ post.url }})
{% endfor %}
