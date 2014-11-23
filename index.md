---
layout: page
title: 紫瞳之仁
tagline: 紫瞳之仁的博客
---
{% include JB/setup %}
<aside id="sidebar" class="alignright">

  <div class="widget tag">
<h4 class="title">基友情深</h4>
<ul class="entry">
<li><a href="http://shhuang.tk/" title="伪文艺黄大腿的窝" target="_blank">伪文艺黄大腿的窝</a></li>
</ul>
</div>
</aside>
{% for post in site.posts %}

<div class = "card">
		<div  class = "date_label">
			<div class="day_month">
      			{{ post.date | date:"%m/%d" }}
      			</div>
      			<div class="year">
      			{{ post.date | date:"%Y" }}
      			</div>
      		</div> 
		{{ post.content  | | split:'<!--break-->' | first }}
	<div class = "read_more">
		<a class="fa fa-link" href="{{ BASE_PATH }}{{ post.url }}">  查看全文&hellip;</a>
	</div>
	
</div>

{% endfor %}

