---
permalink: /
title: "About"
excerpt: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I'm a NASA Postdoctoral Program Fellow at NASA Goddard Space Flight Center working with Drs. Mike McElwain, Josh Schlieder, and Tyler Groff. My current research is focused on high contrast imaging of young exoplanetary systems (primarily with JWST coronagraphic imaging and with data from the Subaru Telescope's SCExAO/CHARIS) toward the goal of better understanding how planetary systems form and evolve.

More broadly, my interests lie in improving the value of data through:

- improvements to data processing and analysis techniques, especially on the software side
- better visualizations for both processing techniques and products to facilitate a better understanding of results (both to laypeople and those in the field)

<p align="center">
  <img src="images/ABAurb.png" alt="Near-infrared mage of the AB Aurigae system showing both its complex spiral-armed disk and the embedded protoplanet, AB Aur b." width="600"/>
</p>

High-contrast imaging studies of planet-forming disks are limited by the tendency of stellar PSF-subtraction techniques to induce significant and variable loss of circumstellar light. To meaningfully test any embedded (proto)planet candidates through morphological or spectral analaysis, this flux loss must first be quantified. Conventionally, full modeling of the circumstellar environment was necesssary to produce even rough approximations of this loss. For many of the more interesting systems (i.e., those with non-axisymmetric features suggestive of unseen planets, such as spiral arms), identifying a synthetic model sufficient to calibrate throughput this way is entirely infeasible.

In a recent work, we presented "Constrained Reference Star Differential Imaging" (Constrained RDI): a class of PSF-subtraction techniques that provides circumstellar throughput near 100%, facilitating identification of embedded exoplanets and enabling more detailed studies of the disks themselves. The schematic below compares the conventional RDI approach (left) to that of our Polarimetry Constrained RDI (PCRDI; right). 

<p align="center">
  <img src="images/rdi_and_pcrdi_explanation.png" alt="RDI and PCRDI schematic" width="550"/>
</p>

In PCRDI, existing polarized intensity images are used to estimate the circumstellar signal contained in the data in order to suppress the oversubtraction that normally occurs. In application to non-axisymmetric protoplanetary disks, this estimate can be directly optimized to reduce signal loss to negligible levels on timescales orders of magnitude faster than those required to model the system instead. Below is an example of this optimization process for synthetic multi-wavelength data containing a simulated spiral-armed disk similar to AB Aurigae's disk (pictured above):

<video width="800" controls>
  <source src="images/constrained_rdi_animation.m4v" type="video/mp4">
</video>

This technique was utilized in the discovery of the protoplanet AB Aurigae b (Currie, Lawson, et al. 2022). Applying PCRDI to multiwavelength SCExAO/CHARIS integral field spectroscopy of AB Aur, we were able to confidently recover the distinct blue color of AB Aur b relative to the surrounding disk (right-most panel; PCRDI in blue, conventional RDI in orange):

![](images/abaur_sb_and_color.png)

The wavelength-averaged result from PCRDI was used in the press releases accompanying the AB Aur b paper (the image of AB Aur featured above).

In application to simulated JWST/NIRCam observations, we also demonstrate that an alternate approach using a fully synthetic disk model as the constraint (Model Constrained RDI or MCRDI) is similarly effective for simpler disk systems that can be modeled. Read the paper in ApJL [here](https://iopscience.iop.org/article/10.3847/2041-8213/ac853b/meta) if you're interested in learning more! We intend to release software supporting application of these techniques for the general public in late 2022.
