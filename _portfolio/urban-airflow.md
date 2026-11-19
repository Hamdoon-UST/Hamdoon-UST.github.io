---
title: "District-scale urban airflow"
excerpt: "Airflow at the scale of an urban district. Figures and a video are not on the site yet."
collection: portfolio
date: 2024-06-01
permalink: /projects/urban-airflow/
---

This page is reserved for work on airflow at the scale of an urban district. A written case study was not in the source material for the site, so this entry does not report methods, a site, or results. Add that text in this file, then add figures and a video in the slots below.

{% include media-slot.html
   path="/images/projects/urban-airflow/figure-1.jpg"
   alt="District-scale airflow, overview"
   label="Figure 1"
   caption="Figure 1. Save the overview image as images/projects/urban-airflow/figure-1.jpg. About 1600 pixels wide fits this column."
%}

{% include media-slot.html
   path="/images/projects/urban-airflow/figure-2.jpg"
   alt="District-scale airflow, detail"
   label="Figure 2"
   caption="Figure 2. Optional detail at images/projects/urban-airflow/figure-2.jpg."
%}

{% include media-slot.html
   alt="Video of district-scale urban airflow"
   label="Video"
   caption="Video slot. Prefer a YouTube or Vimeo embed. A local MP4 goes in files/videos/ and must stay under GitHub’s 100 MB limit."
%}

To show a video, edit the include in `_portfolio/urban-airflow.md`:

```liquid
{% raw %}{% include media-slot.html
   youtube_id="YOUR_YOUTUBE_ID"
   alt="District airflow animation"
   caption="Video. Animation of the district flow."
%}{% endraw %}
```

Or use `vimeo_id="YOUR_VIMEO_ID"`, or `mp4="/files/videos/urban-airflow.mp4"`.
