---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
{% assign sections = site.sections | sort: "order" %}
{% for section in sections %}
  <section>
    {{ section.content | markdownify }}
  </section>
{% endfor %}
