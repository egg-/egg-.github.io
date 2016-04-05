---
title: Repositories
permalink: /repositories/
---

{% for rep in site.github.public_repositories %}
{% if rep.fork == false %}

### {{ rep.name }} <a href="{{ rep.html_url }}" title="{{ rep.name }}"><i class="fa fa-github"></i></a>

{{ rep.description }}

{% endif %}
{% endfor %}
