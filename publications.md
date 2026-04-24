---
layout: page
title: Publications
---
## The size of my ... _academic record_

{% assign pubs_by_year = site.data.publications | group_by_exp: "pub", "pub.journal | split: ' ' | slice: 1, 1 | first" | sort: "name" | reverse %}

{% for year in pubs_by_year %}
  <h3>{{ year.name }}</h3>

  <ul class="list-unstyled">
    {% for pub in year.items %}
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
{% endfor %}
