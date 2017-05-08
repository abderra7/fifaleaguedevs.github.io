---
layout: page
title: Calendar
permalink: /calendar/
---

<ul>
{% for fixture in site.data.calendar.Calendar %}
<li style="margin-bottom: 30px; list-style:none;">
<p><strong>Fixture {{fixture.Jornada}}</strong></p>
<ul style="margin: 10px 0 0 20px;">
{% for match in fixture.Partidos %}
<li style="margin-bottom: 10px; list-style:none;">
{{match.equipoLocal}} (<span style="color:#1756a9;">{{match.psnLocal}}</span>) vs {{match.equipoVisitante}} (<span style="color:#1756a9;">{{match.psnVisitante}}</span>) - <em>Match ID: {{match.id}}</em>
</li>
{% endfor %}
</ul>
</li>
{% endfor %}
</ul>