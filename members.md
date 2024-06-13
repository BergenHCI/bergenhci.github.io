---
title: Members
members:
    - name: "Miroslav Bachinski"
      photo: ""
      desc: ""
    - name: "Frode Guribye"
      photo: ""
      desc: ""
    - name: "Morten Fjeld"
      photo: ""
      desc: ""
    - name: "Pavel Okopnyi"
      photo: ""
      desc: ""
---

# Group members

{% if page.members %}
{% for member in page.members %}

<div class="card" style="width: 18rem;">
    <img src="{{member.photo}}" class="card-img-top" alt="...">
    <div class="card-body">
      <h5 class="card-title">{{member.name}}</h5>
      <p class="card-text">{{member.desc}}</p>
    </div>
</div>

{% endfor %}
{% endif %}