---
layout: kz-page
title: Our operations
permalink: /services/
header:
  title: ""
  image_fullwidth: main.jpg
widgets:
- image: recycling1.jpg
  cols: 4
- image: recycling2.jpg
  cols: 4
- image: recycling3.jpg
  cols: 4

---

There are 3 steps in our recycling operations:

1. Collections and Sorting
* We pick up PET plastic recyclables from businesses, residential estates, hotels and restaurants in Lagos. 
* We currently have 2 locations in Lagos - 1 drop-off location in Oniru and 1 sorting centre in Abule-Egba where we collect, sort and remove the lids and labels of plastic bottles. 

2. Baling
* We compact the plastic recyclables into sizeable bales for resale to manufacturing companies that use recycled plastics.

3. Crushing
* We can also crush the plastic recyclables for resale to manufacturing companies that use recycled plastics.

<div class="row">
  {% for widget in page.widgets %}
    {% assign loopindex = forloop.index | modulo: 3 %}
    <div id="{{ widget.anchor }}">{% include _frontpage-widget.html widget=widget %}</div>
    {% if loopindex == 0 %}
  <hr style="height:1px; visibility:hidden;" /> <!-- Prevents long first column items from pushing new rows to the right -->
    {% endif %}
  {% endfor %}
</div>