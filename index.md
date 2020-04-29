---
---

# Blog Posts

Here are my blog posts

{% for post in site.posts reversed %}
* [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}

{% assign postsByYear = site.posts | group_by_exp:"post", "post.date | date:
'%Y'" %}
{% for year in postsByYear %}
* {{ year.name }}
  {% for post in year.items %}
  * [{{ post.title }}]({{ post.url | relative_url }})
  {% endfor %}
{% endfor %}
