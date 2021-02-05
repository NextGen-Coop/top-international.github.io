---
title: Suppliers
permalink: /suppliers/
layout: collection-page
collection: suppliers
menu: true
---
{% assign this_collection = page.collection %}
{% if site.suppliers %}
  <section class="collection {{ this_collection }}">
  {% for item in site.suppliers %}
    <div class="supplier" id="{{ item.slug }}">
      <h3><a href="{{ item.url | relative_url }}">{{ item.name }}</a></h3>
      {% if item.excerpt %}
        <p>{{ item.excerpt }}</p>
      {% endif %}
      {% if item.request_info %}
        <p>Please contact us for information on {{ item.name }}</p>
      {% else %}
        <p>Product list</p>
      {% endif %}
    </div>
  {% endfor %}
{% endif %}
