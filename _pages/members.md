---
permalink: /members/
title: Level Up Fast Members
sidebar:
  - title: ""
    image: assets/images/logo.png
    image_alt: "Logo"
    text: <b>Level Up Fast</b> is a grass-roots effort in digital upskilling for <b>Covid recovery</b>. Brought to you by colleges, universities and other digital skills providers from North East England.
---

<table>
  <tbody>
    {% for member in site.members %}
    <tr>
      <td>
       <!-- <a href="{{ member.url }}"> -->
       {{ member.name }}
       <!-- </a> -->
      </td>
<!--
      <td>
        <figure><img src="{{ member.logo }}" width="auto" height="10"></figure>
      </td>
-->
    </tr>
<!--  <p>{{ member.content | markdownify }}</p> -->
    {% endfor %}
  </tbody>
</table>