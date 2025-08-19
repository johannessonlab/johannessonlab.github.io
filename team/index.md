---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

{% include section.html %}

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: researcher, group: current" %}
{% include list.html data="members" component="portrait" filters="role: postdoc, group: current" %}
{% include list.html data="members" component="portrait" filters="role: phd, group: current" %}
{% include list.html data="members" component="portrait" filters="role: bioinformatician, group: current" %}
{% include list.html data="members" component="portrait" filters="role: labtech, group: current" %}
{% include list.html data="members" component="portrait" filters="role: assistant, group: current" %}
{% include list.html data="members" component="portrait" filters="role: intern, group: current" %}
{% include list.html data="members" component="portrait" filters="role: undergrad, group: current" %}
{% include list.html data="members" component="portrait" filters="role: guest, group: current" %}
{% include section.html background="images/banner.jpg" dark=true %}

{% include section.html %}

## Alumni

{% include list.html data="members" component="portrait" filters="group: alum" style="small" %}

### Undergraduate students & visitors
<ul style="list-style: none;">
  {% for person in site.data.students %}
      <li><b>{{ person.name }}</b> ({{ person.level }})</li>
  {% endfor %}
</ul>

## Funding

{% capture content %}
[![Bergianska stiftelsen](/images/funding_logos/bergianska.png)](https://www.bergianska.se/)

[![Vetenskapsrådet](/images/funding_logos/vr.png)](https://www.vr.se/)

[![Carl Tryggers stiftelse](/images/funding_logos/CTS_logotyp.svg)](https://www.carltryggersstiftelse.se/)

[![LKAB Kiruna](/images/funding_logos/LKAB_logo_blue.svg)](https://lkab.com/en/)

{% endcapture %}

{% include grid.html content=content %}
