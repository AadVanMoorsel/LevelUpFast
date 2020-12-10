---
name: Gateshead College
logo: /assets/images/logogatesheadcollege.png
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

{% if row["Institution"] == "Gateshead College" %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}

{% endif %}

  {% endfor %}
</table>
