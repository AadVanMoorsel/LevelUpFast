---
name: Newcastle University
logo: /assets/images/logonewcastleuniversity.png
---

<h1> Newcastle University</h1>
<table>
  {% for row in site.data.provision %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

{% if row["Institution"] == "Newcastle University" %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}

{% endif %}

  {% endfor %}
</table>
