# **Super-resolution Maps of Solar Magnetic Field**

State of the art deep neural networks to calibrate and super-resolve historical maps of the solar magnetic field.

### Introduction

Over the past 50 years, a variety of instruments have obtained images of the Sun’s magnetic field (magnetograms) to study its origin and evolution. While improvements in instrumentation have led to breakthroughs in our understanding of physical phenomena, differences between subsequent instruments such as resolution, noise, and saturation levels all introduce inhomogeneities into long-term data sets. This poses a significant issue for research applications that require high-resolution and homogeneous data spanning time frames longer than the lifetime of a single instrument.

In this challenge, we aimed to understand if learning-based super-resolution techniques can be applied to images of the Sun’s magnetic field to cross-calibrate instruments. This is important for a number of reasons:

1. A homogeneous observational baseline is critical for understanding the evolution of solar magnetism, space weather, and space climate. 

2. Differences in resolution, spectral inversion techniques, and other instrument specifics prevent direct comparison of magnetograms across instruments over the last 50 years. 

3. Calibration and homogenisation of magnetograms remains an unsolved problem today and traditional approaches can’t solve it.


### Results

This work demonstrates that learning-based super-resolution techniques can successfully up-sample and homogenize solar magnetic field images obtained by two space-based instruments. We demonstrate the suitability of our approach by up-sampling and calibrating MDI magnetograms to the characteristics of HMI, and further propose a set of metrics to evaluate the quality of (1) instrument cross-calibration, and (2) super-resolution of magnetograms that can also be applied across disciplines.

---

