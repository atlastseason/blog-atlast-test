---
# front matter tells Jekyll to process Liquid
title: Home
---

{{"Hello World!" | downcase}}

{% assign image_files = site.static_files | where: "image", true %}
{% for myimage in image_files %}
   ![{{myimage.basename}}]({{myimage.path}} "{{myimage.basename}}")
{% endfor %}
