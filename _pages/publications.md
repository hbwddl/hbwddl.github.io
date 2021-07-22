---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

Publications
------
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

Current Projects
------

* Movement modeling and spatial risk mapping project with Lance Waller

* Statistical consulting for preliminary work on <u><a href="https://www.wired.com/story/could-a-tree-signal-if-a-corpse-is-decaying/">this</a></u> project (detecting decaying bodies using plants). 
