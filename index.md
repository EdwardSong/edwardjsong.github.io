---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---
{% assign post = site.posts.first %}
<h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
({{ post.date | date: '%B %d, %Y' }})
<div>{{ post.content }}</div>

<h1>Posts</h1>
<ul>
    {% for post in site.posts offset:1 limit:5 %}
    <li>
        <a href="{{ post.url }}">{{ post.title }} - ({{ post.date | date: '%B %d, %Y' }})</a>
        <br/>
        {{ post.description }}
    </li>
    {% endfor %}
</ul>