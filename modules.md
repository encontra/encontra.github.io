---
title: Modules
layout: default
---

<table>
{% for module in site.data.modules %}
<tr>
<td><a href="http://github.com/encontra/{{ module.project }}">{{module.name}}</a></td>
<td>{{module.description}}</td>
<td>
  <a href="https://encontra.ci.cloudbees.com/job/{{ module.project }}">
   <img src="https://encontra.ci.cloudbees.com/buildStatus/icon?job={{ module.project }}">
   </a>
</td>
</tr>
{% endfor %}
</table>
