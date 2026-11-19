---
title: "Hemisphere–cylinder vortex dynamics"
excerpt: "Unsteady leeward vortices on a hemisphere–cylinder at high Reynolds number."
collection: portfolio
date: 2022-07-06
permalink: /projects/hemisphere-cylinder/
---

This project is the vortex flow over a hemisphere–cylinder body when the boundary layer separates as a turbulent flow. It is reported in two journal articles with Bao-Feng Ma, the second also with Peixin Dong.

In the 2022 study we simulated a body of fineness ratio 24.5 with detached-eddy simulation at angles of attack from 30° to 80°. The Reynolds number based on cylinder diameter was fixed at

$$\mathrm{Re}_D = 3.0 \times 10^{6}.$$

Dynamic mode decomposition was used to separate the unsteady motion. Below about 45° the downstream wake moved only weakly, and in phase, unlike the laminar-separation cases in earlier literature. Above about 45° the flow split into slower forebody vortex oscillation and faster shedding from the aft body. The oscillation produced the larger sectional side force. At 50° the leading oscillatory mode was antisymmetric. From 50° to 80°, shedding frequencies along the aft cylinder collapsed approximately onto one line when they were scaled by the cross-flow speed normal to the axis. The oscillation frequencies did not follow that scaling.

The 2026 study asks whether that drop in oscillation frequency is caused by the aft-body shedding. Large-eddy simulations at 30° and 50°, across several fineness ratios, still show forebody oscillation after the aft body is shortened enough that shedding disappears. The frequency change is a property of the forebody vortices. Shortening the aft body changes their amplitude and frequency only slightly, and slightly downward.

* <a href="https://doi.org/10.1063/5.0095746">Ijaz and Ma, Physics of Fluids 34, 077105 (2022)</a>
* <a href="https://doi.org/10.1063/5.0352022">Ijaz, Ma, and Dong, Physics of Fluids 38, 118108 (2026)</a>

{% include media-slot.html
   path="/images/projects/hemisphere-cylinder/figure-1.jpg"
   alt="Hemisphere-cylinder geometry and surface flow"
   label="Figure 1"
   caption="Figure 1. Geometry or surface flow. Save it as images/projects/hemisphere-cylinder/figure-1.jpg (about 1600 pixels wide)."
%}

{% include media-slot.html
   path="/images/projects/hemisphere-cylinder/figure-2.jpg"
   alt="Dynamic mode of the leeward vortices"
   label="Figure 2"
   caption="Figure 2. A mode or wake view at images/projects/hemisphere-cylinder/figure-2.jpg."
%}

{% include media-slot.html
   alt="Video of hemisphere-cylinder vortex motion"
   label="Video"
   caption="Video slot. Add youtube_id, vimeo_id, or mp4 on the include in this file. See the wave-metamaterials page for copy-paste examples, and HOW_TO_ADD_CONTENT.md for file-size limits."
%}
