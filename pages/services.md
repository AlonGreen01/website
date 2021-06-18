---
layout: kz-page
title: Our services
permalink: /services/
header:
  title: ""
  image_fullwidth: main.jpg
widgets:
- title: What we do
  text: "&#8226; We collect waste streams and incentivize<br/>&#8226; We sort the recyclables<br/>&#8226; We bail the recyclables<br/>&#8226; We sell the recyclables"
  image: big_logo.jpg
  cols: 6
- title: How we do it
  text: "&#8226; Recyclables pickup from schools <br/>&#8226; Communities/estates, corporates, drive, eateries, event centers<br/>&#8226; Recyclables drop off at companies<br/>&#8226; Corporate pickup to help reduce their waste footprint"
  image: plastic_collect.jpg
  cols: 6

---

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>
