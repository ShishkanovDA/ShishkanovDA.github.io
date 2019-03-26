---
layout: default
title: news
---
{% for post in site.categories.news %}

<div class="blog-post">
        <h2 class="blog-post-title"><a href="{{ post.url|prepend: site.baseurl }}">{{ post.title }}</a></h2>
		<time class="post_date">{{ post.date | date: "%d %B %Y, %A" }}</time>
		{{ post.content }}
</div>

{% endfor %}
