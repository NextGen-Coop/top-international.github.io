---
title: Suppliers & Products
permalink: /suppliers-products/
layout: collection-page
collection: suppliers
menu: true
---
{% assign this_collection = page.collection %}
{% if site.suppliers %}
  <section class="collection {{ this_collection }}">
  {% for item in site.suppliers %}
    <div class="supplier" id="{{ item.uuid }}">
      <h3><a href="{{ item.url | relative_url }}">{{ item.name }}</a></h3>
      {% if item.excerpt %}
        <p>{{ item.excerpt }}</p>
      {% endif %}
      {% if item.request_info %}
        <p>Please contact us for information on {{ item.name }}</p>
      {% else %}
        {% if site.products %}
          {% include product-list.html supplier=item.uuid %}
        {% endif %}
      {% endif %}
    </div>
  {% endfor %}
{% endif %}
