---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
pagination: 10
---

{% for post in site.posts %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
{% if post.modified %}
<p>{{ post.modified | date: "%-d %B %Y" }}</p>
{% elsif post.date %}
<p>{{ post.date | date: "%-d %B %Y" }}</p>
{% endif %}
<p>{{ post.excerpt | markdownify }}</p>
{% endfor %}
