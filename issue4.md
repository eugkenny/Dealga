---
layout: page
title: Volume 4, 2021
permalink: /issue4/
---

<ul id="archive">
{% for paper in site.data.issue4 %}
  <li class="archiveposturl">
    <!-- <span><a href="{{ site.baseurl }}/{{ issue.title }}">{{issue.title}}</a></span><br> -->
    {% if paper.notes != null %}
      <span class = "postlower"><b>{{paper.notes | upcase}}</b></span><br>
    {% endif %}
   
    <span>{{paper.author | upcase}}: </span>
    <a href="{{ site.baseurl }}/{{paper.dirname}}{{paper.filename}}">
    <span>{{paper.title}}</span></a><br>
   
    <strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right; padding-right: .5em"> </strong>
  </li>
{% endfor %}
</ul>
