---
title: "Numerical modeling of the magnetic field distribution in single-phase single-core transformer"
date: 2019-02-28T23:22:41+02:00
draft: false
dropCap: false
description: "An electromagnetic model of single-phase single-core transformer is made and a numerical simulation of the electromagnetic field is performed"
# featuredImage: "img/20190228-featuredImage-   "
featuredImageDescription: "img/20190228"
displayInMenu: false
categories: ["Modeling", "Papers", "Simulation"]
tags: ["electromagnetic interference", "numerical modelling", "magnetic induction", "transformer"]
displayInList: true
---

An electromagnetic model of single-phase single-core transformer is made and a numerical simulation of the electromagnetic field is performed. 
The distribution of the magnetic induction in the transformer's core and in the surrounding space is obtained. 
A comparative analysis of the obtained electromagnetic values with the computed parameters by a chain model is carried out. 
The investigation enables the determination of the magnetic flux dissipated in the surrounding space outside the transformer that generates the electromagnetic interference.

# Content

- Introduction
- Theoretical statement
- Numerical modeling
- Conclusions
- References

## Introduction

- Low power transformer P = 250VA 
- Transformer's magnet made of 0.35 mm thick silicon steel sheets
- Circular copper conductors for primary and secondary winding
- Primary winding - voltage 220V, d=1mm, 289 turns 
- Secondary winding - voltage 72, d=1.62mm, 104 turns 

The purpose of the study is the distribution of the magnetic field of a single-phase single-core transformer.
The characteristics of the investigated transformer are shown in the slide
Power of the transformer is (two hundred fifty) 250VA,
magnet made of 0.35 mm thick silicon steel sheets, 
circular copper conductors 
With d1=1mm and (two hundred eighty nine) 289 turns for the primary winding and
104 (one hundred and four) turns with conductor diameter of 1.62
Others: The low power transformer P = 250VA with, primary voltage U1=220V (two hundred twenty) and secondary voltage U2=72V is investigated.
The transformer's magnet is made of 0.35 mm thick silicon steel sheets. 
The primary winding is made of a circular copper conductor of diameter d1= 1.0mm  and with W1 = 289 turns.
The secondary winding is made of a circular copper conductor of diameter d2 = 1.62 mm and with  W2 = 104 turns.

## Theoretical statement

The electromagnetic field in the transformer is described with a Poisson‘ equation

The current density is non-zero only in the cross-section of the winding.

The current in the primary winding is 

$i_1(t) = i_m \sin  \omega t$, where $i_m$ is the amplitude, and $\omega$ is the angular frequency of the current in the primary winding.

The primary coil is connected to a sinusoidal voltage source with a frequency $f = 50 Hz$.

The current density in the primary winding $J_1$ is 

$ J_1 = ( N_1/S_1 ) * i_m sin \omega t $, where $N_1$ is the number of turns of the primary winding and $S_1$ is the cross-section of the primary winding

The current density in the secondary winding is $J_1 = (N_2/S_2) * i_2(t)$
Where $N_2$ is the number of turns of the secondary winding
- $S_2$ is the cross-sectional area of the secondary winding
- $I_2(t)$ is the current through the secondary winding.

The magnetic field in the transformer is flat-parallel, magnetostatic in a non-homogeneous environment and therefore the task as a two-dimensional one can be solved.

The all area of the study is divided into two parts - an area of the magnet core and the windings, where the magnetic field is concentrated and an area of the air, where the magnetic field is scattered.

Due to the symmetry of the transformer design, only half of the transformer can be tested.

The magnetic vector-potential has the component only on the z-axis - $A_z$
since the current density through the windings is in the z-axis direction – $J_z$

Figure 1. The schema of the investigated transformer

![Figure 1. The schema of the investigated transformer](/posts-content/2019-02-28-num-modeling-of-the-magn-field-in-single-phase-single-core-transf/fig1-investigated-transformer.png)

## Numerical modeling

Numerical modeling is done using the finite element method FEM.
The ANSYS software package is used.

Figure 2. Distribution on magnetic induction in magnetic core.
![Figure 2. Distribution on magnetic induction in magnetic core.](/posts-content/2019-02-28-num-modeling-of-the-magn-field-in-single-phase-single-core-transf/fig2-dist-on-magnetic-induction-in-core.png)


Figure 3. Distribution magnetic flux lines in magnetic core.
![Figure 3. Distribution magnetic flux lines in magnetic core.](/posts-content/2019-02-28-num-modeling-of-the-magn-field-in-single-phase-single-core-transf/fig3-dis-magn-flux-lines-in-core.png)

Fig. 4 Distribution magnetic flux lines in magnetic core and air zone by idle mode.
![Fig. 4 Distribution magnetic flux lines in magnetic core and air zone by idle mode.](/posts-content/2019-02-28-num-modeling-of-the-magn-field-in-single-phase-single-core-transf/fig4-magnetic-flux-lines-in-core-and-air-zone-by-idle-mode.png)

Fig. 5 Distribution of magnetic vector-potential by idle mode.
![Fig. 5 Distribution of magnetic vector-potential by idle mode.](/posts-content/2019-02-28-num-modeling-of-the-magn-field-in-single-phase-single-core-transf/fig5-dist-of-magn-vector-potential-by-idle-mode.png)

Fig. 6 Distribution on 2-D flux lines by short circuit mode.
![Fig. 6 Distribution on 2-D flux lines by short circuit mode.](/posts-content/2019-02-28-num-modeling-of-the-magn-field-in-single-phase-single-core-transf/fig6-dist-on-2d-flux-lines-by-short-circuit-mode.png)

Fig. 7 Distribution on magnetic induction vectors by short circuit mode.
![Fig. 7 Distribution on magnetic induction vectors by short circuit mode.](/posts-content/2019-02-28-num-modeling-of-the-magn-field-in-single-phase-single-core-transf/fig7-dist-on-magnetic-induc-vectors-by-short-circ-mode.png)

## Conclusions

As a conclusions
An electromagnetic model of single-phase single-core transformer is made and a numerical simulation of the electromagnetic field is performed. 
The distribution of the magnetic induction in the transformer's core and in the surrounding space is obtained.
The investigation enables the determination of the magnetic flux dissipated in the surrounding space outside the transformer that generates the electromagnetic interference.

## References

The full content of this article can downloaded and read from the following url:

[Numerical modeling of the magnetic field distribution in single-phase single-core transformer](/posts-content/2019-02-28-num-modeling-of-the-magn-field-in-single-phase-single-core-transf/2019-02-28-num-modeling-of-the-magn-field-in-single-phase-single-core-transf.pdf)
