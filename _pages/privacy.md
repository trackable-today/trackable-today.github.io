---
layout: page
title: Privacy Policy
include_in_header: false
---

**Last updated**  
August 7 2023

{% for section in site.data.privacy %}
{% if section.hidden %}
{% elsif section.header == site.data.privacy[0].header %}

# {{section.header}}
{{section.text}}

{% else %}

### {{section.header}}
{{section.text}}

{% endif %}
{% endfor %}
