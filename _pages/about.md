---
permalink: /
title: "About"
excerpt: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I am an assistant research scientist working at NASA Goddard Space Flight
Center (through a CRESST-II appointment at the University of Maryland,
Baltimore County). I study exoplanetary systems through high-contrast imaging,
with a particular focus on data post-processing methods and the planetary
systems of low mass stars. Currently, my time is split between two research
projects. 

In the first project, I'm working with high-contrast imaging data from JWST.
This includes further development of <a
href="https://github.com/kdlawson/Winnie/"><tt>Winnie</tt></a>, a Python
package for post-processing and analysis of circumstellar disk systems that I
created during my time as a NASA Postdoctoral Program fellow. As part of this
project, I will also be working with observations from a JWST Cycle 4 program
that I led (GO 8826), which will observe a sample of 22 very nearby young M
dwarfs to search for exoplanets and debris disks. 

<p align="center">
<video width="500" controls>
  <source src="images/abaur_deconv_anim.mov" type="video/mp4">
</video>
</p>
<em>Deconvolution of simulated JWST NIRCam coronagraphic observations of the AB
Aurigae protoplanetary disk system using <tt>Winnie</tt>. NIRCam's shaped pupil produces
a complicated blurring pattern that otherwise all but precludes detailed study
of disk structure. <tt>Winnie</tt>'s deconvolution procedure corrects for this blurring 
to make such studies possible.</em>

<p align="center">
  <img src="images/STScI_jwst_aumic_press_release.png" alt="Press release for Lawson et al. (2023)" width="1200"/>
</p>
<em>Press release images of the AU Microscopii debris disk at 3.6 and 4.4 microns as observed by JWST/NIRCam (reported in Lawson et al. 2023).</em>

In the second project, I am developing a framework to enable the discovery of
exoplanets and debris disks in planned survey observations from the Roman Space
Telescope's Wide Field Instrument (WFI). The significantly undersampled PSF
(FWHM ~ 1.2 pix at 1.6 microns) makes this task especially challenging from the
perspective of conventional post-processing methods, as any sub-pixel
interpolations (e.g., to align stellar PSFs for subtraction) will lead to image
artifacts that prohibit high-contrast sensitivity. However, fundamentally,
these data should be capable of high-contrast performance comparable to HST's
NICMOS (or better). While NICMOS was limited to observing a single star at a time (~400
stars total), WFI's High Latitude Wide Area Survey (HLWAS) will observe ~40000
stars within 100 pc (and many millions of stars at larger distances). While
these data will require novel post-processing methods, such efforts are
well-motivated by the unbelievably massive scale of the sample. 

Before coming to Goddard, I worked with observations from the Subaru
Telescope’s SCExAO/CHARIS instrument. As part of this work, I created the
spectropolarimetry data reduction pipeline and also developed post-processing
algorithms to enable discoveries like AB Aurigae b, a candidate disk-embedded
protoplanet. 