---
layout: page
title: Archive
permalink: /archive/
---

<ul id="archive">
{% for issue in site.data.archive %}
  <li class="archiveposturl">
    <span><a href="{{ site.baseurl }}/{{ issue.href }}">{{issue.title}}
    {% if issue.notes != null %}
      <b>: {{issue.notes}}</b>
    {% endif %}
    </a></span><br>
    <span class = "postlower"></span>
    <strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right; padding-right: .5em"> </strong>
  </li>
{% endfor %}
</ul>
