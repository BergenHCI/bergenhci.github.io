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
    {% include member_card.html member=member | markdownify %}
{% endfor %}
{% endif %}