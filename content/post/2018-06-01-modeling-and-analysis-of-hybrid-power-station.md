---
title: "Modelling and analysis of hybrid power station"
date: 2018-06-01T10:10:10+02:00 
draft: false
dropCap: false
description: "Simulation model of hybrid power station containing Photovoltaic and wind generator sources as well as energy storage."
# featuredImage: "img/20190228-featuredImage-   "
featuredImageDescription: "img/20190228"
displayInMenu: false
categories: ["Modeling", "Papers", "Simulation"]
tags: ["analysis", "modelling", "hybrid power station", "photovoltaic plant", "wind-generator", "MATLAB", "harmonics"]
displayInList: true
---

The power station with renewable generating sources is considered. It consist of Photovoltaic plant and Wind-generator. A model of hybrid power station in MATLAB is created. Simulations of the power station operation have been carried out in different modes. The performance of hybrid power station is analysed. The harmonic composition of the generated AC voltage with an industrial frequency is investigated.

## Content

- Introduction
- Description of the hybrid power station
- Model of the hybrid power station
- Simulation results
- Discussion and Conclusion
- References

## Introduction

First of all I want to talk about the key features of the renewable and hybrid sources and how we can take advantage of it.
A convenient, cost-effective and reliable power supply is an essential factor in the development of any area.
There are several ways by which electricity can be generated locally using renewable sources such as solar, wind, biogas, etc.
At present, standalone solar photovoltaic and wind systems have been promoted around the globe on a comparatively larger scale.
These independent systems cannot provide continuous source of energy, as they are seasonal.
Therefore, suitable energy storage systems will be required for these systems in order to satisfy the power demands.
Usually storage system is expensive and the size has to be reduced to a minimum possible for the renewable energy system to be cost effective.
The cost effective solution would be hybrid power systems which can reduce energy storage requirements and of course more reliable and continuous power source

## Description of the hybrid power station

Configuration structure for hybrid system based solar and wind energy sources.

Fig.1 Configuration of Hybrid Energy System.

![Fig.1 Configuration of Hybrid Energy System](/posts-content/2018-06-01-modeling-and-analysis-of-hybrid-power-station/fig1-configuration-of-hybrid-energy-system.png)

Figure 1 show the configuration structure for hybrid system based solar and wind energy sources.
The hybrid power station is consist two reenable sources of small power (10kW) PV plant and wind generator.
Тhe power station is not connected to a distribution grid and power system supplied the AC loads.
To store the generated electricity in the case of  an absence of generating power, a rechargeable battery is used.
The transformation of the produced energy with DC-AC inverter is carried out.
To restrict and optimize charging and battery discharge processes a controller is used.

The hybrid power generation system using wind and solar power includes the following subsystem: solar array, wind turbine, charge controller, battery bank and inverter.

### PV plant

It consists of an arrangement of several components, including solar panels.
Solar panels are used to convert solar radiation to the electrical energy.
Solar panel is a group of a several monocrystalline silicon(mono-Si) modules electrically connected in series parallel combination to generate the required current and voltage.
The electrical power of PV plant is 10 kW, its efficiency is 15.75% and the area of the solar collectors is 63.5 square meters. Тhe generated electricity per year is 10 MWh [3].

### Wind turbine

Wind turbine is that system which extracts energy from wind by rotation of the blades of the wind turbine. The wind turbine is of the vertical type. The power generated from wind is not continuous its fluctuating. А wind turbine data and electricity generation from the wind turbine using RETScreen Expert software tool [6] are calculated. They are presented in Figure 4 and Figure 5, respectively.

### Charge controller

Charge controller has basic function is that it control the source which is to be active or inactive. It simultaneously charge battery and also gives power to the load. The controller has over-charge protection, short-circuit protection, pole confusion protection and automatic dumpload function. It has also the function, which it should vary the power as per the load demand. It add the both the power so that the load demand can fulfill. When power is not generating the controller should extract power from battery and give it to the load.

### Battery Energy Storage System (BESS)

DC power Batteries are charged and discharged in different mode.
Bidirectional power electronic devices are regulating power flow between batteries and energy systems [4].

### Inverter

Inverter is need to convert DC power into AC power. As our load working on the AC supply so we need to convert DC power. The input voltage, output voltage and frequency, and overall power handling depends on the design of the specific device or the circuitry. The pure sign wave inverter is recommended, because it has minimal distortion and loses.

## Model of the hybrid power station

The entire system design of the hybrid energy system.
A 10-kW PV / Wind / BESS (Battery Energy Storage System) hybrid system.

Fig. 6 Block diagram of the simulated Hybrid Power Station

![Fig. 6 Block diagram of the simulated Hybrid Power Station](/posts-content/2018-06-01-modeling-and-analysis-of-hybrid-power-station/fig6-block-diagram-of-the-simulated-hybrid-power-station.png)

The entire system design of the hybrid energy system is simulated using SIMULINK.
A 10-kW PV / wind / BESS (Battery Energy Storage System) hybrid system was considered.
Figure 6 show the simulation schematic for hybrid station with solar and wind sources.
All the energy sources are modelled using MATLAB [7] software tool to analyse their behavior.
An easy control technique tracks the maximum power from the solar / wind energy source to accomplish much higher generating capacity factors.
The simulation results prove the feasibility and reliability of this proposed system.

## Simulation results

Several simulation of the operation and conditions of the hybrid power plant are carried out.
The different simulations are presented in the slide
As you can see for Simulation 1, there are different whether conditions for both pv and wind sources
For simulation 2 – the pv plant produce max power, while no wind power is generated
Simulation 3 – there is max wind power, but no solar energy is generated
Simulation 4 and 5 the hybrid power station generates 60% of its capacity, while the first simulation more of the power comes from the wind, and the second simulation from photovoltaic plan

Common conditions
The load demand to fulfil is 10 KW throughout the time scale except at 4 to 5 sec when it increases to 14 KW.
Battery initial state-of-charge 60%.

- Simulation 1 - Case of variable weather conditions
Solar energy drops its irradiance from 100% to 25 % from 2 sec.
Wind turbine initially rotating at 5m/s excels to base speed 12m/s after 0.5 sec.
Its rotating speed is decreased to 25 % of its base speed
- Simulation 2 - Maximum solar energy, while no wind power – 100% pv 0% wind
- Simulation 3 - maximum wind power, while no solar energy (0%, 12 m/s)
- Simulation 4 - Power station works with 60% of the installed power – 20% pv 40% wind
- Simulation 5 - Power station works with 60% of the installed power – 40% pv 20% wind

## Simulation results

### Simulation 1, Case of variable weather conditions

The simulation results of voltages and currents in the three phases, and voltage and current in battery in this case are shown in Figure 7 and Figure 8, respectively.

Fig. 7 Voltages and currents in the three phases
![Fig. 7 Voltages and currents in the three phases](/posts-content/2018-06-01-modeling-and-analysis-of-hybrid-power-station/fig7-voltages-and-currents-in-the-three-phases.png)

Fig. 8 Voltages and currents in the battery
![Fig. 8 Voltages and currents in the battery](/posts-content/2018-06-01-modeling-and-analysis-of-hybrid-power-station/fig8-voltages-and-currents-in-the-battery.png)

Fig. 9 Generated Wind power and PV power in Wats
![Fig. 9 Generated Wind power and PV power in Wats](/posts-content/2018-06-01-modeling-and-analysis-of-hybrid-power-station/fig9-generated-wind-ppower-and-pv-power-in-wats.png)

Fig. 10 Harmonics analysis with two sources
![Fig. 10 Harmonics analysis with two sources](/posts-content/2018-06-01-modeling-and-analysis-of-hybrid-power-station/fig10-harmonics-analysis-with-two-sources.png)

## Conclusion

The electric power can be utilize where it generated so that it will reduce the transmission losses and cost.
There are several ways by which electricity can be generated using renewable sources such as solar, wind, biogas, etc. Individual generation of solar and wind energy is costlier.
The using the non conventional energy resources is highly safe for the environment as it doesn’t produce any emission and harmful waste product like conventional energy resources. It is cost effective solution for generation. It only need initial investment.
Cost reduction can be done by increasing the production of the equipment and stimulate our economy by creating jobs in the manufacturing and installation of solar and wind energy systems.
By using solar and wind integrated system we can electrify remote area, also in future it is applicable in smart grid to for metro cities avoid unwanted load shedding.
Solar and wind energy integrated technologies have great potential.

## References

The full content of this article can downloaded and read from the following url:

[Modeling and analysis of hybrid power station](/posts-content/2018-06-01-modeling-and-analysis-of-hybrid-power-station/2018-06-01-modeling-and-analysis-of-hybrid-power-station.pdf)
