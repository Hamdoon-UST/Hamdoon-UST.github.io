---
permalink: /
title: "Hamdoon Ijaz"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a Ph.D. student at The Hong Kong University of Science and Technology. My doctoral research is on the control of shallow-water waves with metamaterials.

I completed an M.Eng. in Aeronautical Science and Engineering, with a specialization in fluid mechanics, at Beihang University, and a B.Sc. in Mechanical Engineering at COMSATS University Islamabad. Before starting the Ph.D. I worked as a research and development engineer at Obrien Tech Limited in Hong Kong. Published work with collaborators includes unsteady vortex flows on hemisphere–cylinder bodies, compound open-channel flow, nanofluid cooling, geotechnical data mapping, and fault-tolerant flight control.

Current research themes:

<ul class="research-themes">
  <li><a href="{{ '/projects/wave-metamaterials/' | relative_url }}">Controlling water waves using metamaterials</a></li>
  <li><a href="{{ '/projects/hemisphere-cylinder/' | relative_url }}">Vortex dynamics of bluff bodies</a></li>
  <li><a href="{{ '/projects/urban-airflow/' | relative_url }}">District-scale urban wind environment & thermal comfort</a></li>
  {% for post in site.portfolio %}
    {% if post.url contains "/projects/nanofluid-radiators" %}
  <li class="research-theme-card">
    <a href="{{ post.url | relative_url }}">
      {% if post.header.teaser %}
      <img src="{{ post.header.teaser | prepend: '/images/' | relative_url }}" alt="Total temperature in a copper oxide–water nanofluid at a Reynolds number of 2,000. Panels, from top to bottom, are 0.5%, 1%, and 1.5% copper oxide by volume, on a scale from 300 to 307.">
      {% endif %}
      <span>{{ post.title }}</span>
    </a>
  </li>
    {% endif %}
  {% endfor %}
</ul>

Please write to <a href="mailto:hijaz@connect.ust.hk">hijaz@connect.ust.hk</a> if you would like to discuss this work.

## Representative Publications

Representative papers are listed below. The complete list is on the [publications page]({{ '/publications/' | relative_url }}). My name is marked in bold.

{::nomarkdown}
{% include representative-publications.html %}
{:/nomarkdown}
