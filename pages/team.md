---
layout: kz-page
title: Our team
permalink: /team/
header:
  title: ""
  image_fullwidth: main.jpg
widgets:
- title: Dolapo Olusanmokun
  text: "Dolapo is a development economist with over ten years experience working on economic growth programmes in East and West Africa across agriculture, health and waste management sectors. Dolapo is enthusiastic about how best African urban cities can create job opportunities within the waste management sector and tap into other circular economy opportunities to improve livelihoods. Dolapo is the CEO of Alon Green Recycling."
  image: team1.jpg
  cols: 6
- title: Adewale Badmos
  text: "Adewale is an agile enterprise developer and project manager with 6 years of experience leading teams and projects across tech, renewable energy, recycling and non-profit. He is a growth hacker and advocates for youth leadership. He has been president of AIESEC where he grew his local chapter and increased Alumni Participation. Adewale is good at making connections and leveraging that connection to build growth. Adewale currently manages Alon Green Recycling operations."
  image: team2.jpg
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

