---
title: "Simulation of sinusoidal voltage inverter using reducing switching losses PWM strategy"
date: 2016-09-15T10:10:10+02:00
draft: false
dropCap: true
description: "The article examines the work of a converter that synthesizes sinusoidal voltage supply to the active-inductive load through method of controlled high-frequency pulses with sinusoidal pulse-width modulation."
# featuredImage: "img/20190228-featuredImage-   "
featuredImageDescription: "img/20190228"
displayInMenu: false
categories: ["Modeling", "Papers", "Simulation"]
tags: ["simulation", "converter", "PWM", "power losses", "model", "SIMULINK"]
displayInList: true
---

The article examines the work of a converter that synthesizes sinusoidal voltage supply to the active-inductive load through method of controlled high-frequency pulses with sinusoidal pulse-width modulation.
High frequency semiconductor key elements of the converter switched at zero current, i.e. with reduced switching losses, each high-frequency pulse transmitted to the load range specified quantity / dose / energy.
The linear dependence on active power in load to the first harmonic amplitude of load voltage and regulation angle respectively is achieved. Simulations on the operation of the converter to achieve a sinusoidal voltage in the converter output are carried out.
Simulink model of the investigated converter is composed.

## Content

- Introduction
- Model of the sinusoidal voltage invertor
- Analysis of the sinusoidal voltage invertor
- Results of simulation
- Conclusion

## Introduction

Pulse width modulation PWM is used in a variety of applications including sophisticated control circuitry.
PWM is used in many industrial mostly for controlling the voltage of the DC/AC converters using the full bridge mode PWM feature.
PWM been widely used for control of AC motors.
The main advantage of PWM is that power loss in the switching devices is very low.
When a switch is off there is practically no current, and when it is on and power is being transferred to the load, there is almost no voltage drop across the switch.
Power loss, being the product of voltage and current, is thus in both cases close to zero.

## Model of the sinusoidal voltage invertor

The circuit model of the studied sine voltage inverter is shown in below, Fig.1 Circuit model of the studied invertor
![Fig.1 Circuit model of the studied invertor](/posts-content/2016-09-15-simul-of-sin-volt-inv-using-reducing-switching-losses-pwm-strategy/circuit-mode-of-the-studied-invertor.png)

The first step in this work was to create the model of the inverter.
The circuit model of the studied sine voltage inverter is shown in Fig. 1.
In this case the studied system consists of the following blocks: high-frequency inverter, switch, filter-load.

The high-frequency inverter includes elements:

- power source E;
- switching (dispensing) capacitors $𝐶_1$ and $𝐶_2$ ($𝐶_1$ = $𝐶_2$);
- switching inductance $𝐿_𝑘$;
- transistors $𝑇_1$ and $𝑇_2$;
- reverse diodes $𝐷_1$ and $𝐷_2$;
- dosing diodes $𝐷_3$ and $𝐷_4$.

The commutator consists of a

- bridge rectifier diode $𝐷_5$÷$𝐷_8$ and
- bridge inverter (IGBT modules $𝑇_3$÷$𝑇_6$ and the corresponding set diodes diode - $𝐷_9$÷$𝐷_12$).

The inverter operates at a voltage load frequency of 50Hz.

The filter contains the elements:

- inductance $𝐿_𝑓$;
- capacitors $𝐶_𝑓$ and $𝐶_𝑓1$, respectively.

Active-inductive load (elements R and L) connects via a separating transformer to the converter.

## Analysis of the sinusoidal voltage invertor

The processes in the scheme of converter described by system of IDE[^1].
[^1]: IDE: Integro-differential equation

The processes in the scheme of converter (Fig 1) for the moment, in which the transistor $T_1$ is opened, a $T_2$ is clogged and operates one of the pairs IGBT (Insulated-gate bipolar transistor)  modules ($T_3$, $T_4$ or $T_5$, $T_6$) are described by system of integral-differential equations.

## Results of simulation

Fig.3 Voltages and currents in commutated transistor T1 and T2 in HFI
![Fig.3 Voltages and currents in commutated transistor T1 and T2 in HFI](/posts-content/2016-09-15-simul-of-sin-volt-inv-using-reducing-switching-losses-pwm-strategy/fig3-voltages-and-currents-in-commutated-t1-and-t2-in-hfi.png)

Fig.4 Transient process for forming of the sinusoidal voltage
![Fig.4 Transient process for forming of the sinusoidal voltage](/posts-content/2016-09-15-simul-of-sin-volt-inv-using-reducing-switching-losses-pwm-strategy/fig4-transient-process.png)

The Simulink model consists of high-frequency inverter, commutator, separating transformer, filter, active-inductive load and control block.
The high-frequency inverter contains of power source; the models switching (dispensing) capacitors, switching inductance, transistors, reverse diodes and dosing diodes.
The commutator contains models of bridge rectifier and bridge inverter.
The filter contains the elements: inductance and filtering capacitors for alternative current and first harmonic of voltage.
The simulations are performed at different parameters of load (resistance and inductance) and different power of consumer.
The nominal full power of investigated inverter is $600 VA$. The load connected to the output is changed from pure active to active-inductive.
Voltages $𝑢_𝐺𝑇1$, $𝑢_𝐺𝑇2$ and currents $𝑖_𝐺𝑇1$, $𝑖_𝐺𝑇2$, obtained from a high-frequency pulse generator, are shown in fig. 3.
Transient process for forming of the sinusoidal voltage in load are shown in fig. 4

The currents in filtering inductance $𝐿_𝑓$ and capacitance $𝐶_𝑓$

Fig.5 Graphics of currents in filtering inductance $𝐿_𝑓$ and capacitance $𝐶_𝑓$
![Fig.5 Graphics of currents in filtering inductance 𝐿_𝑓 and capacitance 𝐶_𝑓](/posts-content/2016-09-15-simul-of-sin-volt-inv-using-reducing-switching-losses-pwm-strategy/fig5-graphics-of-currenmts-in-filtering-inductance-and-cap.png)

The currents in filtering inductance $𝐿_𝑓$ and capacitance $𝐶_𝑓$ are shown in fig.5. They are not pure sinusoidal.
If it does not provide for additional measures to eliminate of harmonics, investigated inverter will not correspond to the highest requirements for electromagnetic compatibility, provided in Bulgarian and International standards for this class of devices.
As a result of mutual compensation of inductance and capacitance and the action of the additional smoothing function of the separating transformer of the inverter output current through the load is sinusoidal.
The obtained almost of an ideal sinusoidal voltage trough active-inductive load and output current in divided transformer are shown in Fig. 6.

## Conclusion

Proven the capabilities of the inverter for the synthesis of sinusoidal output voltage

Fig.6 Sinusoidal voltage trough active-inductive load and output current in divided transformer

![Fig.6 Sinusoidal voltage trough active-inductive load and output current in divided transformer](/posts-content/2016-09-15-simul-of-sin-volt-inv-using-reducing-switching-losses-pwm-strategy/fig6-sin-voltage-through-active-ind-load-and-output-current-in-dev-transf.png)

The simulation model of the sinusoidal voltage invertor is created.
As a result of the analysis and simulations, obtained through the program package MATLAB 7.1 is proven the capabilities of the inverter for the synthesis of sinusoidal output voltage.
Obtaining of an ideal sinusoidal voltage leads to a significant reduction of harmonics in the load of the converter. This ensures low level of electromagnetic interference and improves electromagnetic compatibility.
Switching semiconductor elements of high-frequency inverter is performed at zero current, by using high-frequency current impulses, controlled by SPWM signal.
The energy supplied from the high-frequency inverter in the process of synthesizing of the sinusoidal output voltage is dosed. By this dosing, the power losses in the power controllers, divided transformer and filtering inductance are minimal.
The analysis and simulations allows determining the parameters of the sinusoidal mode in blocks of control and filter-load.

## References

The full content of this article can downloaded and read from the following url:

[Simulation of sinusoidal voltage inverter using reducing switching losses PWM strategy](/posts-content/2016-09-15-simul-of-sin-volt-inv-using-reducing-switching-losses-pwm-strategy/2016-09-15-simulation-of-sin-voltage-inverter.pdf)
