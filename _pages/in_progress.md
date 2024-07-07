---
layout: archive
title: "Works In Progress"
permalink: /in_progress/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}


{% for post in site.in_progresss | reverse %}
	  {% include archive-single.html %}
{% endfor %}
