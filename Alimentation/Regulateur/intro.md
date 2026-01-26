# Introduction

## Objective

The goal of the following notebooks is to provide reference code for designing both voltage **stabilizers** and **regulators**.

The main difference between the two lies in the presence of a feedback loop:

* A *stabilizer* does **not** include feedback.
* A *regulator*, on the other hand, uses a **feedback loop** to improve the stability and accuracy of the output voltage.

## Motivation

These circuits are particularly useful in fields such as **metrology**, where output components can be highly sensitive to input voltage variations and require a very stable supply.
However, such circuits also appear in many other engineering domains whenever stable and reliable voltages are needed.

## Structure of the Notebooks

* [**Voltage Divider**](./Pond_diviseur_tension)
  Although not a stabilizer or a regulator, the voltage divider is a fundamental introduction to voltage-conditioning circuits.
  The goal is to derive its equations and, more importantly, to highlight its limitations.

* [**Series Voltage Stabilizer**](./Diode_Zener)
  This notebook introduces a basic stabilizer using a Zener diode and a series transistor.
  We derive the key equations and discuss the limits of this approach.

* [**Series Voltage Regulator with Control Transistor**](./regulateur_tension_serie_transistor_2)
  Here, we add a feedback loop using a transistor.
  The objective remains the same: understand the equations and see how the circuit can be improved.

* [**Series Voltage Regulator with Operational Amplifier**](./regulateur_tension_serie_AOP_2)
  This section pursues the same goals as the previous one, but replaces the feedback transistor with an **operational amplifier**, enabling higher performance and finer control.