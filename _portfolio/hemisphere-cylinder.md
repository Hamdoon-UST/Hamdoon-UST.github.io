---
title: "Vortex Dynamics of Bluff Bodies"
excerpt: "I used computational fluid dynamics (CFD) to study how vortices form and move around a cylinder with a hemispherical nose."
collection: portfolio
date: 2022-07-06
permalink: /projects/hemisphere-cylinder/
---

I used computational fluid dynamics (CFD) to study how vortices form and move around a cylinder with a hemispherical nose. At a 30° angle of attack, the vortices oscillated weakly and the side force stayed close to zero. At higher angles, the vortices over the front of the body oscillated more strongly, while vortices shed from the rear. By comparing flow animations with force measurements from the simulations, I examined how these changes in the flow affected the sideways loading on the body.

{% include media-slot.html
   path="/images/projects/hemisphere-cylinder/vortex-oscillation-shedding.jpg"
   width="100%"
   alt="Two panels. Left: a simulation of a long rounded-nose body covered in blue, green, yellow, and red vortical structures, with arrows marking vortex oscillation (VO) near the nose and vortex shedding (VS) farther downstream. Right: a photograph of an aircraft at high angle of attack, with a pale cloud of vapour streaming along the fuselage."
   label="Figure 1"
   caption="Figure 1. Vortex oscillation and shedding. The simulation on the left shows two regions: vortex oscillation (VO) near the nose and vortex shedding (VS) farther downstream. The aircraft photograph on the right provides a visual analogy for the flow at high angle of attack."
%}

<figure class="media-slot-row">
{% include media-slot.html
   mp4="/files/videos/hemisphere-cylinder/small-oscillations.mp4"
   alt="Animation of a flow cross-section. A circular body sits beneath a pair of vortices drawn with dense streamlines, one on each side of the centreline. The pair shifts only slightly."
   label="Figure 2 video"
%}
{% include media-slot.html
   path="/images/projects/hemisphere-cylinder/forces-aoa-30.jpg"
   alt="Line chart titled alpha equals 30 degrees, with time in seconds on the horizontal axis. The legend shows C_z total in red, C_y total in blue, and C_x total in green. The red line stays near zero, the blue line stays near 0.55, and the green line stays just above zero."
   label="Figure 2 force plot"
%}
<figcaption>Figure 2. Small oscillations at 30° · Sectional video and force plot. The video shows weak motion of the vortex pair in a cross-section of the flow. In the accompanying plot, the total side-force coefficient (red) stays close to zero.</figcaption>
</figure>

<figure class="media-slot-row">
{% include media-slot.html
   mp4="/files/videos/hemisphere-cylinder/aoa-50-oscillations.mp4"
   alt="Animation of a flow cross-section coloured by streamwise X-vorticity, red for positive and blue for negative. Above a circular body, the red and blue regions move from one side of the body to the other. A time readout in seconds is shown."
   label="Figure 3 video"
%}
{% include media-slot.html
   path="/images/projects/hemisphere-cylinder/forces-aoa-45.jpg"
   alt="Line chart titled alpha equals 45 degrees, with time in seconds on the horizontal axis. The legend shows C_z total in red, C_y total in blue, and C_x total in green. The red line swings between large positive and negative values, the blue line stays near 1.4 with small ripples, and the green line stays near zero."
   label="Figure 3 force plot"
%}
<figcaption>Figure 3. Larger oscillations at high angle of attack · Sectional video and force plot. The 50° video shows the forebody vortices moving alternately on either side of the body. The force plot shown here, labelled 45°, illustrates the much larger side-force fluctuations in the high-angle regime.</figcaption>
</figure>

{% include media-slot.html
   mp4="/files/videos/hemisphere-cylinder/three-dimensional-vortices.mp4"
   alt="Three-dimensional animation of a slender body with a rounded nose. Coloured vortical structures run along the body, shifting near the nose and extending downstream. A colour bar for streamwise vorticity and an X-Y-Z axis triad are shown."
   label="Figure 4"
   caption="Figure 4. Three-dimensional vortex motion · Video. The animation follows the vortices along the body, showing how the forebody oscillations seen in cross-section fit into the wider flow and how vortices shed farther downstream."
%}

{% include media-slot.html
   path="/images/projects/hemisphere-cylinder/dmd-m1-aoa-30.jpg"
   width="100%"
   alt="Dynamic mode decomposition figure labelled M1 mode, alpha equals 30 degrees. Three rows are marked x direction (axial), y direction (normal), and z direction (lateral). Each row shows red and blue vortical structures along a slender grey body, with a wider view on the left and a closer view on the right."
   label="Figure 5"
   caption="Figure 5. Vortex oscillation modes · DMD figure. Dynamic mode decomposition (DMD) identifies patterns that repeat in the flow. At 30°, the vortex pair oscillates weakly and in phase. At 50°, the leading mode is antisymmetric: the two forebody vortices oscillate out of phase."
%}

## Related publications

* Hamdoon Ijaz and Bao-Feng Ma (2022). [Unsteady vortex flows around a hemisphere–cylinder body with turbulent separation](/publication/hemisphere-cylinder-turbulent-separation) ([https://doi.org/10.1063/5.0095746](https://doi.org/10.1063/5.0095746)). *Physics of Fluids*, 34, 077105. <a href="/files/papers/hemisphere-cylinder-turbulent-separation.pdf">[PDF]</a>
* Hamdoon Ijaz, Bao-Feng Ma, and Peixin Dong (2026). [Effects of aftbody vortex shedding on forebody vortex oscillation over hemisphere–cylinder bodies](/publication/aftbody-vortex-shedding) ([https://doi.org/10.1063/5.0352022](https://doi.org/10.1063/5.0352022)). *Physics of Fluids*, 38, 118108. <a href="/files/papers/aftbody-vortex-shedding.pdf">[PDF]</a>
