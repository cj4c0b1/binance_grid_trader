# Changelog

{% for version, date, sections in versions %}
## {{ version }} ({{ date }})

{% for section_name, section_items in sections.items() %}
### {{ section_name }}

{% for item in section_items %}
- {{ item }}
{% endfor %}

{% endfor %}
{% endfor %}
