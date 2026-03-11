---
layout: default
title: "Welcome to Duck Improv"
---

<h1>Welcome to Duck Improv</h1>

{% for post in site.posts %}
  <article style="margin-bottom: 50px;">
    <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
    <p style="color: gray; font-size: 0.9em;"><em>{{ post.date | date: "%B %d, %Y" }}</em></p>
    
    <div>
      {{ post.content }}
    </div>
  </article>
  <hr>
{% endfor %}