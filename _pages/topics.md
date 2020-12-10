---
permalink: /topics/
title: Digital Safety Provision
sidebar:
  - title: ""
    image: assets/images/logo.png
    image_alt: "Logo"
    text: <b>Level Up Fast</b> is a grass-roots effort in digital upskilling for <b>Covid recovery</b>. Brought to you by colleges, universities and other digital skills providers from North East England.
---

<table>
  {% for row in site.data.provision %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}

  {% endfor %}
</table>