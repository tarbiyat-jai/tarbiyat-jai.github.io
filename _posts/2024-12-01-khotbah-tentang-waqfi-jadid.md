---
layout: post
title: "Khotbah Jum'at mengenai Waqfi Jadid"
categories: khotbah
---

<table>
<tr>
    <th>Tanggal</th>
    <th>Judul</th>
</tr>
{% assign tema_khusus = "waqfi-jadid" %}

{% for item in site.data.khotbah %}
    {% if item.tema contains tema_khusus %}
<tr>
    <td>{{ item.tanggal }}</td>
    <td><a href="{{ item.tautan }}" target="_blank">{{ item.judul }}</a></td>
</tr>
    {% endif %}
{% endfor %}
</table>

