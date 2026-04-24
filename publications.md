---
layout: page
title: Publications
permalink: /publications/
---
## The size of my ... _academic record_

<ul class="list-unstyled">
{% for pub in site.data.publications %}
  <li style="margin-bottom: 2em;">

    <strong>{{ pub.title }}</strong><br>
    {{ pub.authors }}<br>
    <em>{{ pub.journal }}</em><br>

    <div style="margin-top: 0.4em;">

      {% if pub.doi %}
        <a href="{{ pub.doi }}">🔗 DOI</a>
      {% endif %}

      {% if pub.pdf %}
        {% if pub.doi %} | {% endif %}
        <a href="{{ '/assets/files/' | append: pub.pdf | relative_url }}">📄 PDF</a>
      {% endif %}

      {% if pub.code %}
        {% if pub.doi or pub.pdf %} | {% endif %}
        <a href="{{ '/assets/files/' | append: pub.code | relative_url }}">💻 Code</a>
      {% endif %}

      {% if pub.citations %}
        {% if pub.doi or pub.pdf or pub.code %} | {% endif %}
        Citations: {{ pub.citations }}
      {% endif %}

    </div>

  </li>
{% endfor %}
</ul>
