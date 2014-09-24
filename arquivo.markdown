---
layout: default
title: arquivo
---

### Arquivo

Aqui encontra-se uma selecção de todos os artigos posteriores ao lançamento do novo blog. 

Para consultar os mais recentes [siga a ligação.](http://lourencoazevedo.com/arquivo/)

<div class="hfeed">
	<article class="hentry entry">
	  <p>{% for post in site.posts offset %}
          <strong><a href="{{ post.url }}">{{ post.title }}</a></strong>
	      <time datetime="{{ post.date | xmlschema }}">{{ post.date | date: " - %d-%m-%Y" }}</time>
	      
	      <br>
	  {% endfor %}
	</p>
	</article>
</div>