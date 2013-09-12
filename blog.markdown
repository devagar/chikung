---
layout: default 
title: blog
---

<h3>Artigos</h3>

Os 10 artigos mais recentes de um total de mais de 200. Deseja ler mais? Consulte o [arquivo](/arquivo.html). 
<p></p>

<div class="hfeed">
{% for post in site.posts limit:10 %}
	<h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
	<p class="post-meta">{{ post.date | date_to_string }}</p>
	<p class="post-excerpt">{{ post.excerpt | strip_html }}&hellip; (<a href="{{ post.url }}">Ler mais</a>)</p>
	<hr>
{% endfor %}
</div>