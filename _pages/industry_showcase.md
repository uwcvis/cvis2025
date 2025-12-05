---
title: Industrial Showcases
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: https://cvis2021.weebly.com/uploads/5/6/3/0/56308869/background-images/236520036.jpg
permalink: /industrial-showcase
toc: true
---

<div class="feature__wrapper">
  <div style="text-align: center;">
    <div class="archive__item-body">
      <h1>Industrial Showcases</h1>
      <p>We are proud to showcase our industry partners who support CVIS 2025.</p>
      <p>Interested sponsors are encouraged to contact <a href="mailto:{{ site.email }}">{{ site.email }}</a></p>

      <h2 class="archive__item-title">Platinum Sponsors</h2>
      <div style="display: flex; justify-content: center; align-items: center; flex-wrap: wrap; gap: 40px; margin: 30px 0;">
        {% for sponsor in site.data.sponsors.platinum %}
          <div style="text-align: center;">
            <a href="{{ sponsor.url }}" target="_blank">
              <img src="{{ sponsor.image_path | relative_url }}" alt="{{ sponsor.alt }}" title="{{ sponsor.title }}" style="max-width: 300px; max-height: 150px; object-fit: contain;">
            </a>
          </div>
        {% endfor %}
      </div>

      <h2 class="archive__item-title">Gold Sponsors</h2>
      <div style="display: flex; justify-content: center; align-items: center; flex-wrap: wrap; gap: 40px; margin: 30px 0;">
        {% for sponsor in site.data.sponsors.gold %}
          <div style="text-align: center;">
            <a href="{{ sponsor.url }}" target="_blank">
              <img src="{{ sponsor.image_path | relative_url }}" alt="{{ sponsor.alt }}" title="{{ sponsor.title }}" style="max-width: 250px; max-height: 125px; object-fit: contain;">
            </a>
          </div>
        {% endfor %}
      </div>

      <h2 class="archive__item-title">Silver Sponsors</h2>
      <div style="display: flex; justify-content: center; align-items: center; flex-wrap: wrap; gap: 40px; margin: 30px 0;">
        {% for sponsor in site.data.sponsors.silver %}
          <div style="text-align: center;">
            <a href="{{ sponsor.url }}" target="_blank">
              <img src="{{ sponsor.image_path | relative_url }}" alt="{{ sponsor.alt }}" title="{{ sponsor.title }}" style="max-width: 200px; max-height: 100px; object-fit: contain;">
            </a>
          </div>
        {% endfor %}
      </div>
    </div>
  </div>
</div>

