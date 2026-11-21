---
title: "District-scale urban airflow and outdoor thermal comfort"
excerpt: "Airflow at the scale of an urban district. Figures and a video are not on the site yet."
collection: portfolio
date: 2024-06-01
permalink: /projects/urban-airflow/
---

In this project I used computational fluid dynamics (CFD) to study how wind moves through a densely built neighbourhood. I analysed wind speeds along streets, through gaps between buildings, and around towers rising above the surrounding blocks. I compared the wind field with a map of physiological equivalent temperature (PET), an indicator of how outdoor conditions feel to a person. Together, the maps show how wind exposure and thermal comfort can vary over the short distance from a main street to a sheltered space within a block.

{% include media-slot.html
   path="/images/projects/urban-airflow/CAD.png"
   idth="50%"
   alt="Three-dimensional model of the study area, showing street layout, low-rise buildings, and taller towers"
   label="Figure 1"
   caption="Figure 1. Three-dimensional model of the study area. The model captures the street layout, closely spaced low-rise buildings, and several taller towers. Differences in building height and spacing shape the paths available for wind to move through the neighbourhood."
%}
<div class="media-slot-row">
{% include media-slot.html
   path="/images/projects/urban-airflow/Mesh1.png"
   alt="Close-up of the triangular surface mesh on building façades, rooftops, and streets"
   label="Figure 2a"
   caption="Figure 2a. Surface mesh around individual buildings. This close-up shows the triangular mesh across façades, rooftops, and streets. The fine spacing around building edges and in narrow passages helps the simulation resolve local changes in airflow."
%}
{% include media-slot.html
   path="/images/projects/urban-airflow/mesh2.png"
   alt="Plan view of mesh refinement across the district, finest along buildings and streets"
   label="Figure 2b"
   caption="Figure 2b. Mesh refinement across the district. In plan view, the mesh is finest along building footprints and within the street network. The elements gradually increase in size outside the built-up area, concentrating computational effort where the geometry is most detailed."
%}
</div>

{% include media-slot.html
   path="/images/projects/urban-airflow/wind_vel.png"
   alt="Simulated wind speed over the district, with faster flow in broad street corridors"
   label="Figure 3"
   caption="Figure 3. Simulated wind speed. Several broad street corridors carry faster-moving air into the neighbourhood, while many spaces inside the blocks remain sheltered. A local increase in wind speed is visible around the corner of the large building just left of centre."
%}

{% include media-slot.html
   path="/images/projects/urban-airflow/PET.png"
   alt="Outdoor thermal comfort as PET, from 32 to 44 degrees Celsius"
   label="Figure 4"
   caption="Figure 4. Outdoor thermal comfort expressed as PET. The colour scale spans 32–44 °C PET. Lower values follow parts of the broad street corridors, while higher values appear in several sheltered interior spaces. Comparing this map with the wind-speed figure helps identify streets where stronger airflow coincides with lower thermal exposure."
%}
