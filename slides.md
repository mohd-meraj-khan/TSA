---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /sundog.jpg
# some information about your slides (markdown enabled)
title: Thesis Submission Approval Meeting
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: false
pointer: true

slideNumber: true
---

## A Lattice Boltzmann Framework for Simulating Electromagnetic Scattering and Radiation Forces

Mohd Meraj Khan

<div class="text-3.5 mt-10">
  <b>Advisor:</b> Prof. Anubhab Roy <br>
  <b>Co-advisor:</b> Prof. Sumesh P. Thampi
</div>

<div class="mt-5 py-5 text-3.5" >
  Thesis Submission Approval Meeting <br>
  November 13, 2025
</div>

<div class="flex items-center justify-center mt-10">
  <img src="/figures/IITM_Logo.png" alt="" class="h-20 w-20">
</div>

<div class="text-3 mt-10">
  Fluid Mechanics Division, Department of Applied Mechanics and Biomedical Engineering <br>
  Indian Institute of Technology Madras, Chennai, India, 600036
</div>

<div class="abs-br m-1.5 text-2">
  Background image: https://pixabay.com
</div>

---

## Scattering of EM waves in climate studies

<!-- <div v-click="1" class="text-center mt-5">
Scattering of electromagnetic waves in nature
</div> -->

<div v-click="1" class="grid grid-cols-3 gap-15 mt-10">
  <figure class="text-center">
    <img src="/figures/scattering/sky_unsplash.jpg" alt="Image 1" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Blue sky and white cloud
      <div class="text-2">(Source: unsplash.com)</div>
    </figcaption>
  </figure>
  
  <figure class="text-center">
    <img src="/figures/scattering/rainbow_unsplash.jpg" alt="Image 2" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Rainbow
      <div class="text-2">(Source: unsplash.com)</div>
    </figcaption>
  </figure>
  
  <figure class="text-center">
    <img src="/figures/scattering/halo_wgrz.com.png" alt="Image 3" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Sundog and Halo
      <div class="text-2">(Source: wgrz.org)</div>
    </figcaption>
  </figure>
</div>

<div v-click="2" class="grid grid-cols-3 gap-15 mt-10">
  <figure class="text-center">
    <img src="/figures/energy-budget.jpg" alt="Image 1" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Radiation budget
      <div class="text-2">(Source: climatesight.org)</div>
    </figcaption>
  </figure>
  
  <figure class="text-center">
    <img src="/figures/dust_storm.png" alt="Image 2" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Dust storm
      <div class="text-2">(Source: icarda.org)</div>
    </figcaption>
  </figure>
  
  <figure class="text-center">
    <img src="/figures/hydrometeor.jpg" alt="Image 3" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Precipitation
      <div class="text-2">(Source: pexels.com)</div>
    </figcaption>
  </figure>
</div>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---



## Scattering of EM waves in remote sensing applications



<div class="grid grid-cols-2 gap-5 mt-5 justify-center">
  <figure v-click="1" class="flex flex-col items-center text-center">
    <div class="flex justify-center">
      <img src="/figures/aerosol.jpg" alt="Image 1" class="w-3/4 h-auto">
    </div>
    <figcaption class="text-3 mt-2">
      Aerosol in the atmosphere
      <div class="text-2">(Source: wikipedia.org)</div>
    </figcaption>
  </figure>
  
  <figure v-click="2" class="flex flex-col items-center text-center">
    <div class="flex justify-center">
      <img src="/figures/ocean_optics.jpg" alt="Image 2" class="w-3/4 h-auto">
    </div>
    <figcaption class="text-3 mt-2">
      Ocean optics
      <div class="text-2">(Source: wikipedia.org)</div>
    </figcaption>
  </figure>
</div>


<div class="grid grid-cols-2 gap-5 mt-3 justify-center">
  <figure v-click="3" class="flex flex-col items-center text-center">
    <div class="flex justify-center">
      <img src="/figures/soil_moisture.jpg" alt="Image 1" class="w-3/4 h-auto">
    </div>
    <figcaption class="text-3 mt-2">
      Soil moisture
      <div class="text-2">(Source: nasa.gov)</div>
    </figcaption>
  </figure>
  
  <figure v-click="4" class="flex flex-col items-center text-center">
    <div class="flex justify-center">
      <img src="/figures/cloud.jpg" alt="Image 2" class="w-3/4 h-auto">
    </div>
    <figcaption class="text-3 mt-2">
      Cloud composition
      <div class="text-2">(Source: unsplash.com)</div>
    </figcaption>
  </figure>
</div>


<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---


## Scattering by atmospheric ice crystals


<div class="grid grid-cols-2 gap-5 mt-15 justify-center">
  <figure v-click="1" class="flex flex-col items-center text-center">
    <div class="flex justify-center">
      <img src="/figures/cirrus.jpg" alt="Image 1" class="w-auto h-auto">
    </div>
    <figcaption class="text-3 mt-2">
      Optical depth of cirrus cloud
      <div class="text-2">(Source: nasa.gov)</div>
    </figcaption>
  </figure>
  
  <figure v-click="2" class="flex flex-col items-center text-center">
    <div class="flex justify-center">
      <img src="/figures/Ice_crystals.jpeg" alt="Image 2" class="w-auto h-auto">
    </div>
    <figcaption class="text-3 mt-2">
      Size and shape of ice crystals
      <div class="text-2">(Source: wikipedia.org)</div>
    </figcaption>
  </figure>
</div>





<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>



---

## Particle trapping and manipulation using radiation force

<v-drag  pos="852,15,94,_">
<figure class="text-center">
  <img src="/figures/rad_force/paramecium.png" alt="Image 2" class="w-full h-auto">
</figure>
</v-drag>

<div class="relative w-full mt-0">

<div class="absolute grid grid-cols-2 gap-15 place-items-center mt-15 ">
  <figure  class="text-center">
    <video autoplay loop muted class="w-full h-auto">
      <source src="/figures/rad_force/Particl_Trapping_Nobel_2018.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <figcaption class="text-3 mt-2">
      Demonstration of optical trapping using radiation force
      <div class="text-2"> A Ashkin and J M Dziedzic (1989)</div>
    </figcaption>
  </figure>
  
  <figure v-click="1" class="text-center">
    <video autoplay loop muted class="w-full h-auto mt-5">
      <source src="/figures/rad_force/Particl_Manipulation_Nobel_2018.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <figcaption class="text-3 mt-2">
      Radiation forces enabling particle manipulation — the foundation for optical tweezers
      <div class="text-2"> A Ashkin and J M Dziedzic (1989)</div>
    </figcaption>
  </figure>
</div>

</div>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>


---
layout: default
---

## Governing equations and lattice Boltzmann method

<div class="grid grid-cols-2 gap-6 mt-4">

  <!-- Left Column -->
<div class="pl-0">

<div v-click='1' class="text-4" >
<p class="text-lg mb-3">Maxwell's equations</p>

$$
\begin{alignedat}{3}
\nabla \cdot \mathbf{D} &= \rho 
&\quad\quad &
\nabla \times \mathbf{E} &= -\frac{\partial \mathbf{B}}{\partial t} \\[1.2em]
\nabla \cdot \mathbf{B} &= 0
&\quad\quad &
\nabla \times \mathbf{H} &= \mathbf{J} + \frac{\partial \mathbf{D}}{\partial t}
\end{alignedat}
$$
</div>

<div v-click='2' class="text-4" >
<p class="mt-4 ">For linear media</p>
$$
\mathbf{D} = \varepsilon \mathbf{E}, \quad \mathbf{B} = \mu \mathbf{H}
$$
</div>

<div v-click='3' class="text-4" >
<p class="mt-4 ">Boundary conditions at the interface of two media</p>
$$
\begin{array}{cc}
\begin{aligned}
\hat{n} \cdot (\mathbf{D}_{2} - \mathbf{D}_{1}) &= \sigma \\[1.2em]
\hat{n} \times (\mathbf{E}_{2} - \mathbf{E}_{1}) &= 0
\end{aligned}
&
\begin{aligned}
\hat{n} \cdot (\mathbf{B}_{2} - \mathbf{B}_{1}) &= 0 \\[1.2em]
\hat{n} \times (\mathbf{H}_{2} - \mathbf{H}_{1}) &= \mathbf{K}
\end{aligned}
\end{array}
$$
</div>
</div>


<div class="pl-0">
  <!-- Right Column -->


<div v-click='4'>
<p class="text-lg mb-3">Lattice Boltzmann method</p>


<div class="relative w-full mt-0">

<div v-click.hide='6' absolute inset-0 >
<div >
<div class="flex justify-between items-center text-3.5 mt-2">
  <div class="text-center mr-15 ml-10">
    Post collision
  </div>
  <div class="text-center ml-15 mr-15">
    Pre collision
  </div>
</div>

<figure class="text-center item-center my-1">
  <img src="/figures/LBM_Kruger.png" alt="Image 1" class="h-auto">
</figure>


</div>
</div>


<div v-click="6" absolute inset-0  >
<figure class="text-center item-center">
  <video autoplay loop muted class="w-full h-auto">
    <source src="/figures/rad_force/lattice_boltzmann.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</figure>
</div>

</div>


</div>


<div v-click='4' class="abs-br m-2 mr-5 text-2">
  Hauser and Verhey (2017) Timm Kruger (2017)
</div>

</div>

<v-drag v-click="4" v-click.hide='6' pos="476,337,282,_">
<div class="text-3 text-left">
$$
f_i^* (\vec{x}, t) = f_i (\vec{x}, t) + \frac{\Delta t}{\tau} \left[f_i^{eq} (\vec{x}, t) - f_i (\vec{x}, t) \right]
$$
</div>
</v-drag>

<v-drag  v-click="4" v-click.hide='6' pos="767,345,198,_">
<div class="text-3 text-left">
$$
f_i (\vec{x} + \vec{c}_i \Delta t, t + \Delta t) = f_i^* (\vec{x}, t)
$$
</div>
</v-drag>




<v-drag  v-click="5" v-click.hide='6' pos="575,398,318,_">
<div class="text-3 text-left">
$$
{\bf e}_i^{eq} ({\bf r} ,t) = 
    \begin{cases}
      \frac{1}{6}\Big(\mathbf{E} ({\bf r} ,t) -   {\bf c}_i \times \mathbf{H} ({\bf r} ,t) \Big) & \text{if $i \neq 0$}\\
      (\varepsilon_{r} - 1 ) \mathbf{E} ({\bf r} ,t) & \text{if $i = 0$}
    \end{cases},  \\
    {\bf h}_i^{eq} ({\bf r} ,t) = 
    \begin{cases}
      \frac{1}{6}\Big(\mathbf{H} ({\bf r} ,t) +  {\bf c}_i \times \mathbf{E} ({\bf r} ,t) \Big) & \text{if $i \neq 0$}\\
      (\mu_{r} - 1 ) \mathbf{H} ({\bf r} ,t) & \text{if $i = 0$}
    \end{cases},  
$$
</div>
</v-drag>








<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

</div>

---

## Methods to solve Maxwell's equations

<table class="w-full border-collapse border text-center text-3.5 mt-5">
  <thead>
    <tr class="bg-gray-100">
      <th class="border px-3 py-2 text-center font-bold">Method Category</th>
      <th class="border px-3 py-2 text-center font-bold">Method</th>
      <th class="border px-3 py-2 text-center font-bold">Domain</th>
      <th class="border px-3 py-2 text-center font-bold">Applicable Shapes</th>
      <th class="border px-3 py-2 text-center font-bold">Challenges</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="border px-3 py-2" rowspan="2">Series expansion of basis function</td>
      <td class="border px-3 py-2">Mie</td>
      <td class="border px-3 py-2">Frequency domain</td>
      <td class="border px-3 py-2">Sphere, circular cylinder</td>
      <td class="border px-3 py-2"></td>
    </tr>
    <tr>
      <td class="border px-3 py-2">T-matrix</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">Shapes with symmetries</td>
      <td class="border px-3 py-2"></td>
    </tr>
    <tr>
      <td class="border px-3 py-2" rowspan="2">Solves IE at grids</td>
      <td class="border px-3 py-2">DDA</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">Arbitrary shape</td>
      <td class="border px-3 py-2">Size parameter 10 <div class="text-2" style="color: red"> Kahnert (2016) </div> </td>
    </tr>
    <tr>
      <td class="border px-3 py-2">MoM</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">Low accuracy <div class="text-2" style="color: red"> Mishchenko (2014) </div> </td>
    </tr>
    <tr>
      <td class="border px-3 py-2" rowspan="2">Solves PDE at grids</td>
      <td class="border px-3 py-2">FEM</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">Size parameter 10 <div class="text-2" style="color: red"> Mishchenko et. al (2000)  </div> </td>
    </tr>
    <tr>
      <td class="border px-3 py-2">FDTD</td>
      <td class="border px-3 py-2">Time domain</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">Size parameter 20 <div class="text-2" style="color: red"> Kahnert (2016)  </div> </td>
    </tr>
    <tr>
      <td class="border px-3 py-2" colspan="1">Solves particle populations at grids</td>
      <td class="border px-3 py-2"><span v-mark.circle.red="1">Lattice Boltzmann method</span></td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">''</td>
    </tr>
  </tbody>
</table>

<v-drag pos="765,36,155,_">
<div class="text-3 ">
$$
\text{Size parameter}  = 2 \pi \frac{a}{\lambda}
$$
</div>
</v-drag>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---
layout: center

---


### Scattering and Radiation Forces from Curved Surfaces — An Applicability Study  
*(Published in Journal of Applied Physics)*

<div class="opacity-100">
  
### Scattering Benchmarking via Near-to-Far-Field Transformation  
*(Under review in Journal of Computational Physics)*

### Radiation Forces and Torques on Janus Cylinders  
*(Under review in Physical Review E)*

</div>



---
layout: center

---


### Scattering and Radiation Forces from Curved Surfaces — An Applicability Study  
*(Published in Journal of Applied Physics)*

<div class="opacity-10">
  
### Scattering Benchmarking via Near-to-Far-Field Transformation  
*(Under review in Journal of Computational Physics)*

### Radiation Forces and Torques on Janus Cylinders  
*(Under review in Physical Review E)*

</div>



---

## Problem setup for LBM Simulation

<div class="flex justify-center w-full mt-1">
  <div class="w-3/4 h-auto text-center">
    <img src="/figures/scattering_Schematic.png" alt="Image 1" class="mx-auto">
  </div>
</div>





<div class="grid grid-cols-2 gap-10 items-start justify-center mt-0">

  <!-- Left column -->
<div v-click="1" class="flex flex-col items-center text-center gap-4">
<p class="text-lg ">Scattering Width / Radar Cross Section</p>

<div class="text-3">
$$
\sigma_{2D} = \lim_{r \to \infty}\, 2\pi r \,\frac{|{\bf E}^S|^2}{|{\bf E}^I|^2}, \quad \sigma_{3D} = \lim_{r \to \infty}\, 4\pi r^2 \,\frac{|{\bf E}^S|^2}{|{\bf E}^I|^2}
$$
</div>

</div>

<!-- Right column -->
<div v-click="2" class="flex flex-col items-center text-center gap-4">
<p class="text-lg ">Radiation Force and Torque</p>

<div class="text-3">
$$
\langle {\bf F} \rangle
= \oint \langle \mathbb{T} \rangle \cdot \hat{\bf n}\, dl, \quad \langle {\bf M} \rangle
= \oint {\bf r} \times ( \langle \mathbb{T} \rangle \cdot \hat{\bf n} )\, dl
$$
</div>





<div class="text-3 mt-0">
$$
\langle \mathbb{T} \rangle
= \frac{1}{2}\,\Re\!\left[
\varepsilon_0\, {\bf E}{\bf E}^*
+ \mu_0\, {\bf H}{\bf H}^*
- \frac{1}{2}\left(\varepsilon_0 |{\bf E}|^2 + \mu_0 |{\bf H}|^2\right)\mathbb{I}
\right]
$$
</div>
</div>

</div>







<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering and radiation force on a conducting circular cylinder


<div class="grid grid-cols-[35%_65%] gap-5 items-start justify-center mt-0">

  <figure v-click class="text-center mt-5">
    <img src="/figures/RCS_PEC.svg" alt="Image 1" class="w-auto h-full">
  </figure>
  
 
  
  <figure v-click class="text-center mt-30 ml-10">
    <img src="/figures/Fx_PEC1.svg" alt="Image 1" class="w-3/4 h-auto">
  </figure>

</div>


<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>


---

## Scattering from a dielectric circular cylinder

<div v-click="1" class="text-center text-3 mb-0 mt-0">
$$
\varepsilon_r = 2
$$
</div>

<div class="grid grid-cols-3 gap-5 items-start justify-center mt-5">

  <figure v-click='1' class="text-center">
    <img src="/figures/RCS_Rayleigh_er_2.svg" alt="Image 1" class="w-auto h-full">
  </figure>
  
  
  <figure v-click='1' class="text-center">
    <img src="/figures/RCS_Mie_er_2.svg" alt="Image 1" class="w-full h-auto">
  </figure>
  
  <figure v-click='1' class="text-center">
    <img src="/figures/RCS_GO_er_2.svg" alt="Image 1" class="w-full h-auto">
  </figure>
  
</div>


<div v-click="2" class="text-center text-3 mb-0 mt-0">
$$
a/\lambda = 0.5
$$
</div>


<div class="col-span-3 flex justify-center items-center gap-10">
  <figure v-click='2' class="text-center">
    <img src="/figures/BRCS_ratio_0.5.svg" alt="Image 1" class="w-auto h-full">
  </figure>

  <figure v-click='2' class="text-center">
    <img src="/figures/MRCS_ratio_0.5.svg" alt="Image 2" class="w-auto h-full">
  </figure>
</div>



<v-drag v-click="1" pos="678,37,281,_">
<figure class="text-center">
  <img src="/figures/legend.png" alt="Image 2" class="w-full h-auto">
</figure>
</v-drag>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Radiation force on dielectric circular cylinder

<div class="grid grid-cols-3 gap-6 mt-5">
  <figure v-click class="text-center">
    <img src="/figures/FxDielRayleigh.svg" alt="Image 1" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Rayleigh regime
    </figcaption>
  </figure>
  
  <figure v-click class="text-center">
    <img src="/figures/FxDielMie.svg" alt="Image 2" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Mie regime
    </figcaption>
  </figure>
  
  <figure v-click class="text-center">
    <img src="/figures/FxDielGO.svg" alt="Image 3" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Geometrical optics regime
    </figcaption>
  </figure>
  
</div>

<div v-click class="text-3 mt-10">

| $a / \lambda$ | $\varepsilon_r$ | $a / \Delta x$ | $\lambda / \Delta x$ (within scatterer) | Time (seconds) |               $\%$ Error                |
| :-----------: | :-------------: | :------------: | :-------------------------------------: | :------------: | :-------------------------------------: |
|      1.0      |        2        |       15       |  <span v-mark.circle.red="5">10</span>  |      0.98      | <span v-mark.circle.red="6">4.33</span> |
|      1.0      |        4        |       20       |  <span v-mark.circle.red="5">10</span>  |      2.53      | <span v-mark.circle.red="6">3.20</span> |
|      0.9      |        9        |       30       |  <span v-mark.circle.red="5">11</span>  |     10.41      | <span v-mark.circle.red="6">5.19</span> |

</div>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Resonance peak

<div class="grid grid-cols-3 gap-6 mt-5">
  <figure class="text-center">
    <img src="/figures/FxMie_er4.svg" alt="Image 1" class="w-full h-auto">
  </figure>
  
  <figure v-click="1" class="text-center">
    <img src="/figures/Fx_Mie_err.svg" alt="Image 2" class="w-full h-auto">
  </figure>
  
  <figure v-click="2" class="text-center">
    <img src="/figures/Fx_Mie_peaks_0.95.svg" alt="Image 3" class="w-full h-auto">
  </figure>
  
</div>

<div v-click="3" class="relative w-full mt-10">
 
  <div v-click="3" v-click.hide="4" class="absolute inset-0 grid grid-cols-3 gap-6 place-items-center transition-opacity duration-500 opacity-100">
    <figure class="text-center">
      <img src="/figures/trac91_er_4_avg.svg" alt="Image 1" class="w-full h-auto">
    </figure>
    <figure class="text-center">
      <img src="/figures/trac93_er_4_avg.svg" alt="Image 2" class="w-full h-auto">
    </figure>
    <figure class="text-center">
      <img src="/figures/trac95_er_4_avg.svg" alt="Image 3" class="w-full h-auto">
    </figure>
  </div>

  <!-- Second group of images -->
  <div v-click="4" class="absolute inset-0 grid grid-cols-2 gap-6 place-items-center transition-opacity duration-500 opacity-100">
    <figure class="text-center">
      <img src="/figures/MA_er_4.0.svg" alt="Image 4" class="w-full h-auto">
    </figure>
    <figure class="text-center">
      <img src="/figures/energy_er_4.0.svg" alt="Image 5" class="w-full h-auto">
    </figure>
  </div>
</div>



<v-drag v-click="3" v-click.hide="4" pos="180,271,76,_">
<div class="text-3 text-left">
$$
a/\lambda = 0.91
$$
</div>
</v-drag>


<v-drag v-click="3" v-click.hide="4" pos="415,268,176,_">
<div class="text-3 text-left">
$$
a/\lambda = 0.93
$$
</div>
</v-drag>


<v-drag v-click="3" v-click.hide="4" pos="754,269,112,_">
<div class="text-3 text-left">
$$
a/\lambda = 0.95
$$
</div>
</v-drag>




<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Radiation force on corrugated elliptical conducting cylinder

<div class="flex justify-center w-full">
  <div class="w-3/4 h-auto text-center">
    <img src="/figures/JAP/corrugatedSnap.png" alt="Image 1" class="mx-auto">
  </div>
</div>

<div class="flex justify-center w-full mb-1">
  <img src="/figures/JAP/corrugatedPEC.svg" alt="Image 1" class="m-auto">
</div>

<v-drag pos="693,414,105,_">
  <div text-center text-3 border border-main rounded>
    F.G. Mitri (2019)
  </div>
</v-drag>

<v-drag pos="13,333,288,_">
<div class="text-3 text-left">
$$
r = a \left[ \frac{1}{\sqrt{\left( \cos{\phi} \right)^2 + \left(A \sin{\phi} \right)^2}} + d \cos{(N \phi)} \right]
$$
</div>
</v-drag>

<v-drag pos="103,439,76,_">
<div class="text-3 text-left">
$$
A = \frac{a}{b}
$$
</div>
</v-drag>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Sharp edged scatterer

<v-drag pos="225,101,540,_">
<div v-click.hide="1"  class="mt-3">
  <figure class="text-center">
    <img src="/figures/ice_crystal.png" alt="Image 1" class="w-auto h-auto">
  </figure>
</div>
</v-drag>

<div v-click.hide="1" class="abs-bl m-2 text-2">
  Lamb and Verlinde (2011)
</div>

<div class="grid grid-cols-2 gap-0 items-center justify-center mt-10">

  <figure v-click class="flex flex-col items-center justify-center">
    <img src="/figures/hexagonalEzTot.png" alt="Image 1" class="w-full h-auto">
  </figure>
  
  
  <figure v-click class="flex flex-col items-center justify-center">
    <img src="/figures/UHexagon.svg" alt="Image 3" class="w-4/5 h-auto">
  </figure>
  
</div>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Multiple scatterers


Applications in finding effective dielectric constant of composite materials


<div class="grid grid-cols-3 gap-1 place-items-center text-center mt-15">

  <figure v-click class="text-center self-end">
    <img src="/figures/PEC_Multi_Particles.png" alt="Image 1" class="w-full h-auto">
    <figcaption class="text-3">
      Perfect electric conductor
    </figcaption>
  </figure>
  
  <figure v-click class="text-center self-end">
    <img src="/figures/er5_Multi_Particles.png" alt="Image 2" class="w-full h-auto">
    <figcaption class="text-3">
      Dielectric
    </figcaption>
  </figure>
  
  <figure v-click class="text-center self-end">
    <img src="/figures/MA_energy_multi_particles.svg" alt="Image 3" class="w-full h-auto">
    <figcaption class="text-3 mt-5">
      Energy
    </figcaption>
  </figure>
  
</div>


<v-drag pos="514,400,55,_">
<div v-click='2' class="text-3 text-left">
$$
\varepsilon_r = 5
$$
</div>
</v-drag>


<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---
layout: center

---

<div class="opacity-10">

### Scattering and Radiation Forces from Curved Surfaces — An Applicability Study  
*(Published in Journal of Applied Physics)*

</div>
  
### Scattering Benchmarking via Near-to-Far-Field Transformation  
*(Under review in Journal of Computational Physics)*

<div class="opacity-10">

### Radiation Forces and Torques on Janus Cylinders  
*(Under review in Physical Review E)*

</div>



---

## Scattering from a dielectric circular cylinder

Considering size

<div v-click="1" class="text-center text-3 mb-0 mt-0">
  Perfect electric conductor
</div>

<div v-click="1" class="grid grid-cols-3 gap-0 place-items-center mb-0">
  <figure class="text-center">
    <img src="/figures/SW_PEC_Rayleigh.svg" alt="Image 1" class="w-7/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/SW_PEC_Mie.svg" alt="Image 2" class="w-7/8 h-auto">
  </figure>

  <figure class="text-center">
    <img src="/figures/SW_PEC_GO.svg" alt="Image 3" class="w-7/8 h-auto">
  </figure>
</div>

<div v-click="2" class="text-center text-3 mt-0 mb-0">
  Dielectric of dielectric constant
</div>





<div v-click="2" class="relative w-full mt-0">
 
  <div v-click="2" v-click.hide="3" class="absolute inset-0 grid grid-cols-3 gap-0 place-items-center transition-opacity duration-500 opacity-100">
    <figure class="text-center">
      <img src="/figures/SW_polar_er_2_ratio_0.02.svg" alt="Image 1" class="w-7/8 h-auto">
    </figure>
    <figure class="text-center">
      <img src="/figures/SW_polar_er_2_ratio_0.1.svg" alt="Image 2" class="w-7/8 h-auto">
    </figure>
    <figure class="text-center">
      <img src="/figures/SW_polar_er_2_ratio_1.0.svg" alt="Image 3" class="w-7/8 h-auto">
    </figure>
  </div>

  <!-- Second group of images -->
  <div v-click="3" class="absolute inset-0 grid grid-cols-2 gap-6 place-items-center transition-opacity duration-500 opacity-100">
    <figure class="text-center">
      <img src="/figures/SW_polar_er_2_ratio_10.0.svg" alt="Image 4" class="w-7/8 h-auto">
    </figure>
    <figure class="text-center">
      <img src="/figures/SW_polar_er_2_ratio_50.0.svg" alt="Image 5" class="w-7/8 h-auto">
    </figure>
  </div>
</div>








<v-drag pos="578,316,55,_">
<div v-click="2"  class="text-3 text-left">
$$
\varepsilon_r = 2
$$
</div>
</v-drag>

<v-drag pos="36,461,55,_">
<div v-click="2" v-click.hide="3"  class="text-3 text-left">
$$
\frac{a}{\lambda} = \frac{1}{50}
$$
</div>
</v-drag>

<v-drag pos="327,455,55,_">
<div v-click="2" v-click.hide="3" class="text-3 text-left">
$$
\frac{a}{\lambda} = \frac{1}{10}
$$
</div>
</v-drag>

<v-drag pos="76,441,55,_">
<div v-click="3" class="text-3 text-left">
$$
\frac{a}{\lambda} = 10
$$
</div>
</v-drag>


<v-drag pos="810,427,55,_">
<div v-click="3" class="text-3 text-left">
$$
\frac{a}{\lambda} = 50
$$
</div>
</v-drag>


<v-drag pos="862,464,55,_">
<div v-click="2" v-click.hide="3" class="text-3 text-left">
$$
\frac{a}{\lambda} = 1
$$
</div>
</v-drag>


<!--
<v-drag pos="830,74,139,_">
<div v-click="1"  class="text-2.5 text-left">
$$
\min \{ \lambda_{inc}, a \} = 50 \times \Delta x
$$
</div>
</v-drag>
-->



<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering from a dielectric circular cylinder

Considering size


<v-drag pos="402,106,171,_">
<div v-click="1"  class="text-3">
Perfect electric conductor
</div>
</v-drag>



<div v-click="1" class="grid grid-cols-3 gap-0 place-items-center my-0">
  <figure class="text-center">
    <img src="/figures/EzTot_PEC_Real_0.02.svg" alt="Image 1" class="w-full h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/EzTot_PEC_Real_1.0.svg" alt="Image 2" class="w-full h-auto">
  </figure>

  <figure class="text-center">
    <img src="/figures/EzTot_PEC_Real_50.0.svg" alt="Image 3" class="w-full h-auto">
  </figure>
</div>

<div v-click="2" class="text-center text-3 mt-0 mb-0">
  Dielectric constant
</div>

<div v-click="2" class="grid grid-cols-3 gap-0 place-items-center my-0">
  <figure class="text-center">
    <img src="/figures/EzTot_er_2_Real_0.02.svg" alt="Image 4" class="w-full h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/EzTot_er_2_Real_1.0.svg" alt="Image 5" class="w-full h-auto">
  </figure>

  <figure class="text-center">
    <img src="/figures/EzTot_er_2_Real_50.0.svg" alt="Image 6" class="w-full h-auto">
  </figure>
</div>

<v-drag pos="548,313,55,_">
<div v-click="2"  class="text-3 text-left">
$$
\varepsilon_r = 2
$$
</div>
</v-drag>

<v-drag pos="33,297,55,_">
<div v-click="1"  class="text-2.5 text-left">
$$
\frac{a}{\lambda} = \frac{1}{50}
$$
</div>
</v-drag>

<v-drag pos="313,301,55,_">
<div v-click="1"  class="text-2.5 text-left">
$$
\frac{a}{\lambda} = 1
$$
</div>
</v-drag>

<v-drag pos="869,300,55,_">
<div v-click="1"  class="text-2.5 text-left">
$$
\frac{a}{\lambda} = 50
$$
</div>
</v-drag>


<!--
<v-drag pos="830,74,139,_">
<div v-click="1"  class="text-2.5 text-left">
$$
\min \{ \lambda_{inc}, a \} = 50 \times \Delta x
$$
</div>
</v-drag>
-->

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering from a dielectric circular cylinder

Considering dielectric constant

<div v-click="1" class="grid grid-cols-3 gap-0 place-items-center mt-10">
  <figure class="text-center">
    <img src="/figures/SW_er_5_1.svg" alt="Image 1" class="w-6/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/SW_er_10_1.svg" alt="Image 2" class="w-6/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/SW_er_20_1.svg" alt="Image 2" class="w-6/8 h-auto">
  </figure>
</div>

<div v-click="2" class="grid grid-cols-3 gap-0 place-items-center mt-10">
  <figure class="text-center">
    <img src="/figures/EzTot_er_5_Real_1.svg" alt="Image 3" class="w-auto h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/EzTot_er_10_Real_1.svg" alt="Image 4" class="w-auto h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/EzTot_er_20_Real_1.svg" alt="Image 4" class="w-auto h-auto">
  </figure>
</div>



<v-drag pos="152,308,55,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_r = 5
$$
</div>
</v-drag>

<v-drag pos="442,314,55,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_r = 10
$$
</div>
</v-drag>

<v-drag pos="741,311,55,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_r = 20
$$
</div>
</v-drag>


<!--
<v-drag pos="749,79,228,_">
<div v-click="1"  class="text-3 text-left">
$$
\lambda_{\varepsilon_r} = 50 \times \Delta x, \hspace{10pt} L/a = 10
$$
</div>
</v-drag>
-->


<v-drag pos="440,85,55,_">
<div v-click="1"  class="text-3 text-left">
$$
a / \lambda = 1
$$
</div>
</v-drag>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering from a regular hexagonal dielectric cylinder


<div class="relative w-full mt-10">



<div v-click="1" v-click.hide="3"  class="absolute inset-0 items-center justify-center">

  <div v-click="1"  class="grid grid-cols-3 mt-5 gap-2 place-items-center justify-center transition-opacity duration-500 opacity-100">
    <figure class="flex flex-col items-center">
      <img src="/figures/SW_TM_Hexgon_polar_er_1.721_ratio_0.1.svg" alt="Image 1" class="w-7/8 h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/SW_TM_Hexgon_polar_er_1.721_ratio_1.svg" alt="Image 2" class="w-7/8 h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/SW_TM_Hexgon_polar_er_1.721_ratio_10.svg" alt="Image 3" class="w-7/8 h-auto">
    </figure>
  </div>
  <div v-click="2"  class="grid grid-cols-3 mt-10 gap-2 place-items-center justify-center transition-opacity duration-500 opacity-100">
      <figure class="flex flex-col items-center">
        <img src="/figures/SW_TE_Hexgon_polar_er_1.721_ratio_0.1.svg" alt="Image 4" class="w-7/8 h-auto">
      </figure>
      <figure class="flex flex-col items-center">
        <img src="/figures/SW_TE_Hexgon_polar_er_1.721_ratio_1.svg" alt="Image 5" class="w-7/8 h-auto">
      </figure>
      <figure class="flex flex-col items-center">
        <img src="/figures/SW_TE_Hexgon_polar_er_1.721_ratio_10.svg" alt="Image 5" class="w-7/8 h-auto">
      </figure>
  </div>
  
</div>





<div v-click="3"
       class="absolute inset-0 grid grid-cols-3 gap-2 mt-15 place-items-center justify-center transition-opacity duration-500 opacity-100">
    <figure class="flex flex-col items-center">
      <img src="/figures/Ez_Hexagon_TM_Tot_er_1.721_Real_0.1.svg" alt="Final 1" class="w-full h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/Ez_Hexagon_TM_Tot_er_1.721_Real_1.svg" alt="Final 2" class="w-full h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/Ez_Hexagon_TM_Tot_er_1.721_Real_10.svg" alt="Final 3" class="w-full h-auto">
    </figure>
</div>

</div>


<v-drag pos="-24,190,137,_,270">
<div v-click="1"  class="text-3 text-left">
$$
TM^z \text{polarization}
$$
</div>
</v-drag>

<v-drag pos="-14,431,137,_,270">
<div v-click="2" v-click.hide="3"  class="text-3 text-left">
$$
TE^z \text{polarization}
$$
</div>
</v-drag>


<v-drag pos="442,73,90,_">
<div v-click="1"  class="text-3 text-left">
$$
a/\lambda = 1
$$
</div>
</v-drag>


<v-drag pos="737,76,90,_">
<div v-click="1"  class="text-3 text-left">
$$
a/\lambda = 10
$$
</div>
</v-drag>


<v-drag pos="153,75,90,_">
<div v-click="1"  class="text-3 text-left">
$$
a/\lambda = 1/10
$$
</div>
</v-drag>


<v-drag pos="848,47,90,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_r = 1.721
$$
</div>
</v-drag>



<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering from a dielectric sphere


<div class="relative flex flex-col items-center justify-center mt-10">

<figure v-click.hide="1" class="flex flex-col items-center">
  <img src="/figures/3D_schematic.png" alt="Main Figure" class="w-1/2 h-auto">
</figure>

<div v-click="1" class="absolute inset-0 flex flex-col items-center justify-center">
  <div class="grid grid-cols-3 gap-10 place-items-center justify-center transition-opacity duration-500 opacity-100">
    <figure class="flex flex-col items-center">
      <img src="/figures/RCS_Polar_0.02_2_90.svg" alt="Image 1" class="w-7/8 h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/RCS_Polar_0.1_2_90.svg" alt="Image 2" class="w-7/8 h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/RCS_Polar_1_2_90.svg" alt="Image 3" class="w-7/8 h-auto">
    </figure>
    <div class="col-span-3 flex justify-center gap-10 transition-opacity duration-500 opacity-100">
      <figure class="flex flex-col items-center">
        <img src="/figures/RCS_Polar_2_2_90.svg" alt="Image 4" class="w-7/8 h-auto">
      </figure>
      <figure class="flex flex-col items-center">
        <img src="/figures/RCS_Polar_5_2_90.svg" alt="Image 5" class="w-7/8 h-auto">
      </figure>
    </div>
  </div>
</div>

</div>


<v-drag pos="768,33,90,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_r = 2
$$
</div>
</v-drag>


<v-drag pos="184,75,91,_">
<div v-click="1"  class="text-3 text-left">
$$
a / \lambda = 1/50
$$
</div>
</v-drag>

<v-drag pos="442,75,90,_">
<div v-click="1"  class="text-3 text-left">
$$
a / \lambda = 1/10
$$
</div>
</v-drag>

<v-drag pos="717,75,55,_">
<div v-click="1"  class="text-3 text-left">
$$
a / \lambda = 1
$$
</div>
</v-drag>

<v-drag pos="332,302,55,_">
<div v-click="1"  class="text-3 text-left">
$$
a / \lambda = 2
$$
</div>
</v-drag>

<v-drag pos="587,306,55,_">
<div v-click="1"  class="text-3 text-left">
$$
a / \lambda = 5
$$
</div>
</v-drag>


<!--
<v-drag pos="652,76,228,_">
<div v-click="1"  class="text-3 text-left">
$$
\lambda_{\varepsilon_r} = 50 \times \Delta x, \hspace{10pt} L/a = 10
$$
</div>
</v-drag>
-->

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering from a dielectric sphere



<div  class="grid grid-cols-2 gap-5 place-items-center justify-center mt-10 my-15">
  <figure class="flex flex-col items-center">
    <img src="/figures/sphere_er_2_ratio_0.02.svg" alt="Image 1" class="w-full h-auto">
  </figure>

  <figure class="flex flex-col items-center">
    <img src="/figures/sphere_er_2_ratio_0.1.svg" alt="Image 2" class="w-full h-auto">
  </figure>

  <figure class="flex flex-col items-center">
    <img src="/figures/sphere_er_2_ratio_1.svg" alt="Image 3" class="w-full h-auto">
  </figure>

  <figure class="flex flex-col items-center">
    <img src="/figures/sphere_er_2_ratio_5.svg" alt="Image 4" class="w-full h-auto">
  </figure>
</div>



<v-drag pos="53,177,84,_">
<div class="text-3 text-left">
$$
a / \lambda = 1/50
$$
</div>
</v-drag>

<v-drag pos="519,182,80,_">
<div class="text-3 text-left">
$$
a / \lambda = 1/10
$$
</div>
</v-drag>

<v-drag pos="71,359,60,_">
<div  class="text-3 text-left">
$$
a / \lambda = 1
$$
</div>
</v-drag>

<v-drag pos="524,381,59,_">
<div class="text-3 text-left">
$$
a / \lambda = 5
$$
</div>
</v-drag>

<!--
<v-drag pos="652,76,228,_">
<div v-click="1"  class="text-3 text-left">
$$
\lambda_{\varepsilon_r} = 50 \times \Delta x, \hspace{10pt} L/a = 10
$$
</div>
</v-drag>
-->

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---
layout: center

---


<div class="opacity-10">

### Scattering and Radiation Forces from Curved Surfaces — An Applicability Study  
*(Published in Journal of Applied Physics)*

</div>

<div class="opacity-10">
  
### Scattering Benchmarking via Near-to-Far-Field Transformation  
*(Under review in Journal of Computational Physics)*

</div>

### Radiation Forces and Torques on Janus Cylinders  
*(Under review in Physical Review E)*




---
layout: two-cols-header
---

## Scattering from a Janus cylinder

Scattering width

::left::

<figure class="text-center item-center my-5">
  <img src="/figures/Janus_Half_schematic.svg" alt="Image 1" class="w-3/4 h-auto">
</figure>

::right::



<v-drag pos="439,110,471,_">
<div v-click="1" class="mt-3 text-3.5">
$$
E_z^I (r, \phi) = \sum_{m = 0}^{\infty} \alpha_m (-j)^m J_m (k_0 r) \cos{ { m ( \phi - \phi_0) } }
$$
</div>
</v-drag>



<v-drag pos="446,238,500,_">
<div v-click="1" class="mt-3 text-3.5">
$$
E_z^S (r, \phi) = \sum_{m = 0}^{\infty} \left[ B_m \cos{(m \phi)} + D_m \sin{(m \phi)} \right] H_m^{(1)} (k_0 r)
$$
</div>
</v-drag>


<v-drag pos="567,177,219,_">
<div v-click="1"  class="text-3 text-left">
$$
\alpha_m =
\begin{cases}
0, & \text{if } m = 1, \\
0, & \text{otherwise.}
\end{cases}
$$
</div>
</v-drag>

<v-drag pos="526,398,55,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_{r_1} = 5
$$
</div>
</v-drag>

<!--
<v-drag pos="363,491,228,_">
<div v-click="1"  class="text-3 text-left">
$$
\lambda_{\varepsilon_{r_1}} = 50 \times \Delta x, \hspace{10pt} L/a = 10
$$
</div>
</v-drag>
-->

<v-drag pos="593,341,227,_">
<div v-click="1" class="mt-3">
  <figure class="text-center">
    <img src="/figures/Janus/RCS_5.svg" alt="Image 1" class="w-auto h-auto">
  </figure>
</div>
</v-drag>

<v-drag v-click="1" pos="622,75,168,_">
  <div text-center text-3 border border-main rounded>
    Hurd and Sachdeva (1975)
  </div>
</v-drag>


<v-drag pos="684,492,157,_">
<div v-click="1"  class="text-3 text-left">
$$
\theta = \text{scattering angle}
$$
</div>
</v-drag>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Radiation force and torque on a metallo-dielectric Janus cylinder

<!--
<div v-click="1" class="text-center">
Analytical solution (Hurd and Sachdeva 1975)
</div>
-->

<div v-click="1" class="grid grid-cols-3 gap-0 mt-5 ml-15">
  <figure class="text-center">
    <img src="/figures/Fx_LBM_Hurd.svg" alt="Image 1" class="w-7/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/Fy_LBM_Hurd.svg" alt="Image 2" class="w-7/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/Tz_LBM_Hurd.svg" alt="Image 3" class="w-7/8 h-auto">
  </figure>
</div>

<!--
<div v-click="2" class="text-center mt-0">
LBM solutions
</div>
-->

<div v-click="2" class="text-center text-4 mb-0 mt-3">
  Percentage error
</div>

<div v-click="2" class="grid grid-cols-3 gap-0 mt-5 ml-15">
  <figure class="text-center">
    <img src="/figures/Fx_Hurd_Per_Err.svg" alt="Image 1" class="w-7/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/Fy_Hurd_Per_Err.svg" alt="Image 2" class="w-7/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/Tz_Hurd_Per_Err.svg" alt="Image 3" class="w-7/8 h-auto">
  </figure>
  
</div>

<v-drag v-click="1" pos="-25,197,163,_">
<figure class="text-center">
  <img src="/figures/Janus_schematic_PEC.svg" alt="Image 2" class="w-full h-auto">
</figure>
</v-drag>

<!--
<v-drag pos="756,13,169,_">
<div v-click="2"  class="text-3 text-left">
$$
a = 40 \times \Delta x,  \hspace{10pt} L/a = 4
$$
</div>
</v-drag>
-->



<v-drag pos="220,59,53,_">
<div v-click="1"  class="text-3 text-left">
$$
\langle \vec{F}_x \rangle
$$
</div>
</v-drag>

<v-drag pos="482,55,53,_">
<div v-click="1"  class="text-3 text-left">
$$
\langle \vec{F}_y \rangle
$$
</div>
</v-drag>

<v-drag pos="763,56,53,_">
<div v-click="1"  class="text-3 text-left">
$$
\langle \vec{M}_z \rangle
$$
</div>
</v-drag>



<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Radiation force and torque on a dielectric Jaus cylinder

<div v-click="1" class="grid grid-cols-3 gap-2 mt-8 ml-10">
  <figure class="text-center">
    <img src="/figures/Fx_Janus_er_1.svg" alt="Image 1" class="w-7/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/Fy_Janus_er_1.svg" alt="Image 2" class="w-7/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/Tz_Janus_er_1.svg" alt="Image 3" class="w-7/8 h-auto">
  </figure>
</div>

<div v-click="2" class="grid grid-cols-3 gap-2 mt-5 ml-10">
  <figure class="text-center">
    <img src="/figures/Fx_Janus_er_2.svg" alt="Image 1" class="w-7/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/Fy_Janus_er_2.svg" alt="Image 2" class="w-7/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/Tz_Janus_er_2.svg" alt="Image 3" class="w-7/8 h-auto">
  </figure>
</div>




<v-drag pos="200,72,53,_">
<div v-click="1"  class="text-3 text-left">
$$
\langle \vec{F}_x \rangle
$$
</div>
</v-drag>

<v-drag pos="479,73,53,_">
<div v-click="1"  class="text-3 text-left">
$$
\langle \vec{F}_y \rangle
$$
</div>
</v-drag>

<v-drag pos="760,71,53,_">
<div v-click="1"  class="text-3 text-left">
$$
\langle \vec{M}_z \rangle
$$
</div>
</v-drag>

<v-drag pos="21,143,60,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_{r_1} = 1
$$
</div>
</v-drag>

<v-drag pos="22,378,53,_">
<div v-click="2"  class="text-3 text-left">
$$
\varepsilon_{r_1} = 2
$$
</div>
</v-drag>



<v-drag v-click="1" pos="-25,205,139,_">
<figure class="text-center">
  <img src="/figures/Janus_schematic.svg" alt="Image 2" class="w-full h-auto">
</figure>
</v-drag>

<!--
<v-drag pos="663,1,169,_">
<div v-click="1"  class="text-3 text-left">
$$
a = 3
0 \times \Delta x,  \hspace{10pt} L/a = 4
$$
</div>
</v-drag>
-->
<!--
<v-drag pos="436,26,222,_">
<div v-click="1"  class="text-3 text-left">
4 Parallel threads, 35 secs / simulation 18281 simulations,  1 week
</div>
</v-drag>
-->

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Trajectories of Janus cylinder



<div class="grid grid-cols-[35%_65%] gap-8 items-center justify-center mt-8">

  <!-- Left column: Video -->


  <!-- Right column: Equations -->
<div class="flex flex-col items-center text-center space-y-6">

<p class="text-lg mb-2">Instantaneous Force and Torque Balances</p>

<div  class="text-4">
$$
\mathbf{F}^{H} + \mathbf{F}^{EM} = 0, \quad \mathbf{M}^{H} + \mathbf{M}^{EM} = 0
$$

</div>





<p class="text-lg mt-4">Hydrodynamic Resistances</p>

<div  class="text-4">
$$
\mathbf{F}^{H} =
-\frac{4\pi \eta L}{\log(L/a)} \, \mathbf{U}
$$

</div>

<div class="text-4">
$$
\mathbf{M}^{H} =
-4\pi \eta a^{2} \mathbf{\Omega}
$$

</div>

</div>




<div class="flex justify-center items-center mr--25">
<figure class="text-center">
  <video autoplay loop muted playsinline class="w-full h-auto ">
    <source src="/figures/Janus_Trajectories_fixed_er.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  
</figure>
</div>



</div>

  



<v-drag pos="749,26,70,_">
<div  class="text-3 text-left">
$$
\varepsilon_{r_1} = 1
$$
</div>
</v-drag>






<v-drag pos="831,4,141,_">
<figure class="text-center">
  <img src="/figures/Janus_schematic_PEC.svg" alt="Image 2" class="w-full h-auto">
</figure>
</v-drag>




<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Trajectories of Janus cylinder

<div v-click="1" class="grid grid-cols-3 gap-2 mt-5 ml-15">
  <figure class="text-center">
    <img src="/figures/MDJC_Trajectory_er_1.svg" alt="Image 1" class="w-full h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/MDJC_Trajectory_er_3.svg" alt="Image 2" class="w-full h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/MDJC_Trajectory_er_5.svg" alt="Image 3" class="w-full h-auto">
  </figure>
</div>



<v-drag pos="248,253,70,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_{r_1} = 1
$$
</div>
</v-drag>

<v-drag pos="517,255,70,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_{r_1} = 2
$$
</div>
</v-drag>

<v-drag pos="792,255,70,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_{r_1} = 5
$$
</div>
</v-drag>





<div v-click="2" class="grid grid-cols-3 gap-2 mt-10 ml-15">
  <figure class="text-center">
    <img src="/figures/DJC_Trajectory_er_2_er2byer1_2.svg" alt="Image 1" class="w-full h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/DJC_Trajectory_er_2_er2byer1_2.svg" alt="Image 2" class="w-full h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/DJC_Trajectory_er_2_er2byer1_2.svg" alt="Image 3" class="w-full h-auto">
  </figure>
</div>



<v-drag pos="208,468,145,_">
<div v-click="2"  class="text-3 text-left">
$$
\varepsilon_{r_1} = 2, \varepsilon_{r_2} / \varepsilon_{r_1} = 2
$$
</div>
</v-drag>

<v-drag pos="487,469,128,_">
<div v-click="2"  class="text-3 text-left">
$$
\varepsilon_{r_1} = 2, \varepsilon_{r_2} / \varepsilon_{r_1} = 3
$$
</div>
</v-drag>

<v-drag pos="772,475,129,_">
<div v-click="2"  class="text-3 text-left">
$$
\varepsilon_{r_1} = 2, \varepsilon_{r_2} / \varepsilon_{r_1} = 5
$$
</div>
</v-drag>


<v-drag v-click="1" pos="-23,99,141,_">
<figure class="text-center">
  <img src="/figures/Janus_schematic_PEC.svg" alt="Image 2" class="w-full h-auto">
</figure>
</v-drag>

<v-drag v-click="2" pos="-22,319,139,_">
<figure class="text-center">
  <img src="/figures/Janus_schematic.svg" alt="Image 2" class="w-full h-auto">
</figure>
</v-drag>



<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

<!--
## Conclusion






<div class="flex items-start justify-left h-full mt-20">
  <ul class="list-disc text-left">
    <li>Verified LBM's accuracy for electromagnetic scattering and radiation force computations.</li>
    <li>Achieved excellent agreement with analytical results across all scattering regimes.</li>
    <li>Demonstrated efficiency and adaptability for complex geometries.</li>
    <li>Positioned LBM as a reliable tool for computational electrodynamics.</li>
  </ul>
</div>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>
-->

---
class: text-4
---

## Visible research output

| Publications                                                                                                                                                                                                                                 |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1. Electromagnetic scattering by curved surfaces and calculation of radiation force: Lattice Boltzmann simulations <br> <span class="text-3" ><b>Mohd. Meraj Khan</b>, Sumesh P Thampi and Anubhab Roy <i> J. App. Phys. 136, 19</i> </span> |
| 2. Lattice Boltzmann method for electromagnetic wave scattering <br> <span class="text-3" ><b>Mohd. Meraj Khan</b>, Sumesh P Thampi and Anubhab Roy <i> (Under review) J. Comput. Phys </i> </span>                             |
| 3. Radiation Forces and Torques on Janus Cylinders <br> <span class="text-3" ><b>Mohd. Meraj Khan</b>, Sumesh P Thampi and Anubhab Roy <i> (Under review) Phys. Rev. E </i> </span>             |

<div h-3 />

| Code                                                                                                                                                           |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1. Developed an open-source in-house code for scattering and radiation force calculations (<a href="https://github.com/mohd-meraj-khan/LBM-for-scattering" target="_blank">https://github.com/mohd-meraj-khan/LBM-for-scattering</a>) |

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## GitHub repository clone activity



<div class="flex flex-col items-center justify-center my-6">
  <img src="/figures/GitHub_Clones.png" alt="Scattering pattern" class="h-3/4 rounded-xl shadow-lg" />
  <p class="text-sm text-gray-500 mt-3 italic">
    Daily number of unique users who cloned the GitHub repository over the past two weeks.
  </p>
</div>



---
layout: center
class: text-center
---

# Thank you!



<!--
<div class="m-5 text-center">
  <a href="https://github.com/mohd-meraj-khan/LBM-for-scattering" target=_blank>https://github.com/mohd-meraj-khan/LBM-for-scattering</a> 
</div>
-->
