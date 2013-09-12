---
layout: default
title: arquivo
---

### Arquivo

Aqui encontra-se uma selecção de todos os artigos publicados até hoje.

<div class="hfeed">
	<article class="hentry entry">
	  <p>{% for post in site.posts offset %}
	      <time datetime="{{ post.date | xmlschema }}">{{ post.date | date: "%d-%m-%Y - " }}</time>
	      <a href="{{ post.url }}">{{ post.title }}</a>
	      <br>
	  {% endfor %}
	</p>
	</article>
</div>