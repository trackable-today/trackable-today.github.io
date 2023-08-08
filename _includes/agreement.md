
{% for section in agreement %}
{% if section.hidden %}
{% elsif section.header == agreement[0].header %}

# {{section.header}}
{{section.text}}

{% else %}

### {{section.header}}
{{section.text}}

{% endif %}
{% endfor %}
