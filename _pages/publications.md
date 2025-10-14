---
title: Publications
layout: single
permalink: /publications/
collection: publications
---

<ul class="publication-list">
  {% assign pubs = site.publications | sort: 'year' | reverse %}
  {% assign grouped_pubs = pubs | group_by: 'year' %} 

  {% for group in grouped_pubs %}
    <h2>{{ group.name }}</h2>
      {% for pub in group.items %}
        <a href="{{ pub.url | relative_url }}">{{ pub.title }}</a><br>
          {% include publication_entry.html page=pub %}
      {% endfor %}
  {% endfor %}
</ul>
