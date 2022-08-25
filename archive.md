---
layout: page
title: About
---


<p> I'm <a href= "https://www.linkedin.com/in/pippy-stauf-360164249/" >Pippy Stauf</a> listen right here </p>
{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
