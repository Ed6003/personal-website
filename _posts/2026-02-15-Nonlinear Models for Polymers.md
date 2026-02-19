---
title: "Types of Nonlinear Models for Polymers"
date: 2026-02-15
layout: single-custom
entries_layout: grid
pagination:
  enabled: true
tags:
  - "Polymers"
  - "Nonlinear Models"
  - "Simulation"
  - "Materials Science"
author_profile: true
mathjax: true
header:
  particles: true
  overlay_color: "#000"
toc: false
tagline: ""
read_time: true
share: true
related: true
---

Polymers exhibit a wide range of non-linear behaviours under load making their simulation challenging. In contrast to metals, several non-linear behaviours are introduced by large deformations, rate dependence and time-dependance. The main types of non-linear models used to capture polymer behaviour can be broadly divided into hyperelastic models and viscoelastic models.

### 1. Hyperelastic Models

Hyperelastic models are used to describe reversible large deformtions such as in rubbers and elastomers.

$$
W = W(\mathbf{F}) \quad \text{or} \quad W = W(I_1, I_2, I_3)
$$

Hyperelastic models describe the large, reversible deformations typical of rubbers and elastomers. These models use strain energy density functions to relate stress and strain. Common examples include:
- **Neo-Hookean**
- **Mooney-Rivlin**
- **Ogden**
- **Yeoh**
- **Arruda-Boyce**

These models are widely used for soft polymers and biological tissues.

### 2. Viscoelastic Models

$$
\sigma(t) + \tau_\sigma \,\dot{\sigma}(t)
= E_1 \,\varepsilon(t) + E_2 \,\varepsilon(t) + E_2 \tau_\varepsilon \,\dot{\varepsilon}(t)
$$

Viscoelasticity accounts for time-dependent (creep and relaxation) behavior. Linear viscoelastic models use Prony series, but for nonlinear response, models like:
- **Nonlinear Generalised Maxwell**
- **Bergström-Boyce**
- **Schapery’s model**

are used to capture both rate and history dependence.

### 3. Viscoplastic and Elastoplastic Models
Some polymers yield and flow irreversibly under load. Nonlinear viscoplastic models (e.g., Perzyna, Anand) and elastoplastic models (e.g., Drucker-Prager, von Mises with hardening) are used for thermoplastics and filled polymers.

### 4. Damage and Failure Models
To simulate progressive damage, crazing, or fracture, models such as:
- **Continuum Damage Mechanics (CDM)**
- **Cohesive Zone Models (CZM)**
- **Gurson-Tvergaard-Needleman (GTN)**

are applied, especially for predicting failure in toughened polymers and composites.

### 5. Mullins Effect and Hysteresis
For filled rubbers and soft polymers, the Mullins effect (stress softening) and hysteresis are important. Specialized models extend hyperelasticity to capture these phenomena.

---

Choosing the right nonlinear model depends on the polymer type, loading conditions, and the simulation’s goals. Accurate material testing and calibration are essential for reliable results.