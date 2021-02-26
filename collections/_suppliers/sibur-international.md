---
name: Sibur International
uuid: sibur
layout: page
excerpt: A small description of the supplier.
website: https://www.sibur.ru/en/
request_info: true
---
Website: <a href="{{ page.website }}" target="_blank" rel="nofollow">{{ page.website }}</a>

{% include product-list.html supplier=page.uuid %}
