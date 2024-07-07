---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}


{% assign pubs_done = site.publications  |  where: "collection", "publications" %}
{% for post in pubs_done %}
	  {% include archive-single.html %}
{% endfor %}

{% assign in_progress = site.publications | reverse |  where: "collection", "in_progress" %}
{% for post in in_progress %}
	  {% include archive-single.html %}
{% endfor %}
