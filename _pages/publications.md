---
title: Publications
layout: single
permalink: /publications/
collection: publications
---

<ul class="publication-list">
    {% assign pubs = site.publications | sort: 'year' | reverse %}
    {% for pub in site.publications %}
        <a href="{{ pub.url | relative_url }}">{{ pub.title }}</a><br>
        {% include publication_entry.html
             authors=pub.authors
             title=pub.title
             venue=pub.venue
             year=pub.year
             doi=pub.doi %}
    {% endfor %}
</ul>