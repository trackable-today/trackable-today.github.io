---
layout: page
title: Terms Of Use
include_in_header: false
---

**Last updated**  
August 7 2023

{% assign sections = site.data.terms %}

{% for section in sections %}
{% if section.hidden %}
{% elsif section.header == sections[0].header %}

# {{section.header}}
{{section.text}}

{% else %}

### {{section.header}}
{{section.text}}

{% endif %}
{% endfor %}
