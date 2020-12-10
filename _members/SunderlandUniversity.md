---
name: Sunderland University
logo: /assets/images/logosunderlanduniversity.png
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

{% if row["Institution"] == "Sunderland University" %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}

{% endif %}

  {% endfor %}
</table>
