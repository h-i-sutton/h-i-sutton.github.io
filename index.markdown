---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

{% for post in site.posts %}
{% if post.draft %}
{% else %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
{% if post.modified %}
<p>{{ post.modified | date: "%-d %B %Y" }}</p>
{% elsif post.date %}
<p>{{ post.date | date: "%-d %B %Y" }}</p>
{% endif %}
<p>{{ post.excerpt | markdownify }}</p>
{% endif %}
{% endfor %}
