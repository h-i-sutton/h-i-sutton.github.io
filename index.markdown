---
layout: default
---

{% for post in site.posts %}
{% if post.draft %}
{% else %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
<div class="postinfo">#{{ forloop.rindex }}:
{% if post.modified %}
{{ post.modified | date: "%-d %B %Y" }}
{% elsif post.date %}
{{ post.date | date: "%-d %B %Y" }}
{% endif %}
</div>
<p>{{ post.excerpt | markdownify }}</p>
{% endif %}
{% endfor %}
