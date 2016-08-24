---
layout: page
title: Fredy Rincon
---

My GitHub account:
[https://github.com/fredyrincon](https://github.com/fredyrincon)

This is my personal blog, where I'll be posting content related to software engineering.

### Currently learning

- ReactiveUI
- Xamarin Forms
- TravisCI
- Octopus

<br>
<br>
<br>

# Recent articles


{% for post in site.posts limit:4 %}
   <div class="post-preview">
   <h3><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
   <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
   {{ post.content | split:'<!--break-->' | first }}
   {% if post.content contains '<!--break-->' %}
      <a href="{{ post.url }}">Read more</a>
   {% endif %}
   </div>
   <hr>
{% endfor %}