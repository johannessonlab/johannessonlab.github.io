---
title: Team
nav:
  order: 4
  tooltip: About our team
---

# <i class="fas fa-users"></i>Team

Our team is led by professor Hanna Johannesson. We comprise a mix of Swedish and international team members, each with their own unique skillset.

{% include section.html %}

{%
  include list.html
  data="members"
  component="portrait"
  filters="role: pi, group: current"
%}
{%
  include list.html
  data="members"
  component="portrait"
  filters="role: postdoc, group: current"
%}
{%
  include list.html
  data="members"
  component="portrait"
  filters="role: phd, group: current"
%}
{%
  include list.html
  data="members"
  component="portrait"
  filters="role: bioinformatician, group: current"
%}
{%
  include list.html
  data="members"
  component="portrait"
  filters="role: labtech, group: current"
%}
{%
  include list.html
  data="members"
  component="portrait"
  filters="role: guest, group: current"
%}
{:.center}

{% include section.html background="images/banner.jpg" dark=true %}

{% include section.html %}


## Alumni
{%
  include list.html
  data="members"
  component="portrait"
  filters="group: alum"
  style="tiny"
%}

### Undergraduate students & visitors
<ul style="list-style: none;">
  {% for person in site.data.students %}
      <li><b>{{ person.name }}</b> ({{ person.level }})</li>
  {% endfor %}
</ul>


## Funding

Our work is made possible by funding from several organizations.
{:.center}

{%
  include gallery.html

  image1="images/funding_logos/bergianska.png"
  link1="https://www.bergianska.se/"
  tooltip1="Bergianska stiftelsen"

  image2="images/funding_logos/vr.png"
  link2="https://www.vr.se/"
  tooltip2="Vetenskapsrådet"

  image3="images/funding_logos/CTS_logotyp.svg"
  link3="https://www.carltryggersstiftelse.se/"
  tooltip3="Carl Tryggers stiftelse"

  image4="images/funding_logos/LKAB_logo_blue.svg"
  link4="https://lkab.com/en/"
  tooltip4="LKAB Kiruna"
%}
