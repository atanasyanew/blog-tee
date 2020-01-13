---
title: "Performance analysis and modelling of grid-connected small photovoltaic system"
date: 2019-06-06T10:10:10+02:00
draft: false
dropCap: false
description: "The small PV power station, located in Southeast Bulgaria is analysed. Performance analysis of a 30 kW solar photovoltaic power plant is done"
# featuredImage: "img/20190228-featuredImage-   "
featuredImageDescription: "img/20190228"
displayInMenu: false
categories: ["Modeling", "Papers", "Simulation"]
tags: ["electromagnetic compatibility", "harmonic limits", "performance", "power quality", "photovoltaic plant"]
displayInList: true
---

## Abstract

A grid-connected 30 kW small PV system, located in Southeast Bulgaria has been studied.
Performance analysis of the PV system is done.
The PV system is balanced according reactive power.
The total harmonic distortion THD of the object is very low and satisfies the requirements of the standards.
A model of PV system is created in MATLAB.
Simulations of the operation in different modes have been carried out.
The electromagnetic compatibility of analyzed small PV power system is satisfied.

Power station details

- PV modules Polycrystalline silicon TRITEC TRI-MAX EU 250Wp.
- The modules are placed on a support rail with spacing to ensure free flow on air under the modules.
- A string by combination of series connecting modules (6 strings of 20 modules) is formed.
- PV system uses one HUAWEI SUN2000-33KTL - 30 KW.
- The inverter outputs at 400 V, 50 Hz.

Performance analysis

- The performance analysis with apparatus Metrel MI 2392F was conducted. (instruments for power quality analysis)
- For gathering the necessary information, the device is connected to the inverter via L1/2/3 Clamps (clamps 3x300A, range 100%, U range: 240-1000V, L-N, Connection 4W)
- Several measurements are made over a certain time interval, each of 200ms duration and a density of 1024 points

| Fig. 3 Waveforms of voltages and current in normal mode |
|:---:|
| ![Conclusion](/posts-content/2019-06-06-perform-analysis-and-mod-of-grid-connected-pv-system/publication-06-fig-03.png "Conclusion") |

| Fig. 5 Closer view for THD |
|:---:|
| ![Conclusion](/posts-content/2019-06-06-perform-analysis-and-mod-of-grid-connected-pv-system/publication-06-fig-05.png "Conclusion") |

Measurement results

- The shape of the voltage and current are close to the sinusoidal curve.
- The power system is balanced according reactive power.
- Total harmonic distortion is minimal according to IEEE 519

PV System Model

- A model of power system in MATLAB is created.
- A control technique is using to accomplish maximum generating power from the solar plant.
- The results of the simulation prove the stability and reliable operation of the investigated system.
- The investigated PV system using SIMULINK is simulated.
- A 30-kW PV system is considered.

| Fig. 6 Block diagram of the simulated PV system |
|:---:|
| ![Conclusion](/posts-content/2019-06-06-perform-analysis-and-mod-of-grid-connected-pv-system/publication-06-fig-06.png "Conclusion") |

| Fig.8 Simulation result of the voltages in normal mode |
|:---:|
| ![Conclusion](/posts-content/2019-06-06-perform-analysis-and-mod-of-grid-connected-pv-system/publication-06-fig-08.png "Conclusion") |

## Conclusion

The analyzed photovoltaic system has a significant advantage - it reduces the cost of transmission and distribution of electrical energy, because the power is produced with low voltage at the end point of use.
The PV system is balanced according reactive power in normal mode.
This does not obstruct the low voltage distribution grid with the transfer of reactive power.
The total harmonic distortion of the object is very low and satisfies the requirements of the standards.
The electromagnetic compatibility of analyzed small PV power system is satisfied.
