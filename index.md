---
# front matter tells Jekyll to process Liquid
title: Home
---

สวัสดีจ้า นี่คือเว็บบล็อคของมังกรเขียว [atlastseason](https://www.atlastseason.art)

{% assign image_files = site.static_files | where: "image", true %}
{% for myimage in image_files %}
   ![{{myimage.basename}}]({{myimage.path}} "{{myimage.basename}}")
{% endfor %}
