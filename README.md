# −3.5 · How I See

Project page: [anifou.com/project/minus-three-point-five](https://www.anifou.com/project/minus-three-point-five)

---

## Overview

−3.5 (How I See) is a research-based visual simulation exploring how mild to moderate myopia (–3.5 diopters) alters human perception.  

It combines optical physics, perceptual modeling, and neural depth estimation** to recreate the characteristic spatial softness of uncorrected short-sighted vision — not as a blur effect, but as a physiologically consistent image transformation.

Rather than imitating lens defocus in camera space, the system approximates retinal projection and aberration through depth-aware convolution, based on simplified thin-lens geometry and perceptual heuristics.

---

## Concept

The work is situated at the intersection of computational optics, visual neuroscience, and media art.  

It aims to translate an optical condition (myopia) into a reproducible visual logic that can be used for:

- medical communication – explaining refractive phenomena  
- media & design research – perceptual realism in visual systems  
- artistic installations – empathy through altered perception  

---

## Methodological Summary

The simulation is based on a reproducible optical workflow:

1. Depth Estimation – inferred from monocular RGB input via MiDaS / DPT models  
2. Focus Geometry – thin-lens approximation using a –3.5 dpt focal distance (~0.285 m)  
3. Circle of Confusion Mapping – pixelwise CoC derived from focal length, aperture, and focus distance  
4. Aberration Heuristics – perceptual weighting for defocus and astigmatic spread  
5. Depth-dependent Blur Compositing – multi-bin Gaussian blending with optional chromatic shift  

All parameters are normalized for perceptual plausibility rather than diagnostic accuracy.

---

## Ethical & Scientific Position

The project is not a medical diagnostic tool. It visualizes the experience of optical defocus, not its clinical measurement.

- No biometric or personal data is used.  
- All image inputs are public or self-generated.  
- The model is transparent and reproducible in principle, but the full engine is not public.

---

## Repository Scope

This repository contains:
- a technical and conceptual summary of the project  
- sample visual results and comparison images  
- bibliographic and theoretical documentation

The **full simulation engine** (including PSF modeling, Zernike aberrations, and GPU convolution) 
is part of a private research release and is not included here.

For collaborations, academic use, or licensing requests, please contact:

**mail@anifou.com**

---

## References

- Thibos, L. N., Applegate, R. A. et al. (2002). *Standards for reporting optical aberrations of the eye.* J. Refractive Surgery, 18(5).  
- Goodman, J. W. (2005). *Introduction to Fourier Optics.* Roberts & Co.  
- Ranftl, R., Bochkovskiy, A., & Koltun, V. (2021). *Vision Transformers for Dense Prediction.* arXiv:2103.13413  
- Gross, H. et al. (2008). *Handbook of Optical Systems, Vol. 3: Aberration Theory and Correction of Optical Systems.* Wiley-VCH.  

---

© 2025 [**Anifou**](https://www.anifou.com) — All rights reserved.  
