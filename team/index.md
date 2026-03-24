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
[![Kungliga vetenskapsakademien](/images/funding_logos/201501-VA-Webb-Medlemsloggor-12.jpg)](https://www.kva.se/)

[![European Research Council](/images/funding_logos/LOGO-ERC.png)](https://erc.europa.eu/homepage)

[![Vetenskapsrådet](/images/funding_logos/vr.png)](https://www.vr.se/)

[![Crafoordska stiftelsen](/images/funding_logos/crafoord_logo.png)](https://www.crafoord.se/en/)

[![Helge Ax:son Johnsons stiftelse](/images/funding_logos/AxsonJohnsons-2.jpg)](https://www.haxsonj.se/)

[![Olle Engkvists stiftelse](/images/funding_logos/oes-logo.png)](https://https://oes.se/)

[![Sven och Lilly Lawskis fond för naturvetenskaplig forskning ](/images/funding_logos/logo.gif)](https://www.lawskistiftelsen.se/)

[![LKAB Kiruna](/images/funding_logos/LKAB_logo_blue.svg)](https://lkab.com/en/)

{% endcapture %}

{% include grid.html content=content %}
