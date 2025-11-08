# Resume

The first step is to understand what an **amplifier** is and why it is so essential in electronic systems.

## Introduction

An **electronic amplifier** (commonly called an *amplifier* or *amp*) is an electronic system that **increases the power of an electrical signal**.
The additional energy required for amplification is drawn from the amplifier’s **power supply**.

A **perfect amplifier** does not distort its input signal — the output is an **exact replica** of the input, only with a higher amplitude (or, in some cases, a lower impedance).
It is therefore an **active four-terminal network** built around one or more **active components**, most commonly **transistors**.

In an **ideal amplifier**, the relationship between input and output remains **linear** over the entire operating range.

Amplifiers are among the **most important components in analog circuits**, as they allow signals to be properly scaled and conditioned for further processing.
Amplifiers can generally be divided into two major families:

1. **Operational amplifiers (Op-Amps)** – widely used in analog signal conditioning and filtering.
2. **Power amplifier classes** – such as **Class A, B, AB, C, D, and E**, each optimized for a specific efficiency and application.

## Operational Amplifiers (Op-Amps)

Operational amplifiers are one of the **simplest and most versatile** amplifier configurations.
They form the basis of countless analog circuits, including filters, comparators, and signal conditioners.

However, it’s important to note that **op-amps are not optimized for efficiency**.
Their purpose is to provide **high precision and linearity**, not power output — making them ideal for **low-power analog signal processing** rather than energy amplification.

## Power Amplifier Classes

The following sections describe the main **amplifier classes**, each representing a different **operating mode** for the active component (typically a transistor).
These classes trade off **linearity**, **efficiency**, and **distortion**, depending on the desired application.

### Class A

* **Principle:**
  The transistor conducts **continuously (100% of the time)**, even when no signal is applied.

* **Advantages:**

  * Excellent **linearity** → very low distortion
  * **High-fidelity** output (commonly used in high-end audio)

* **Disadvantages:**

  * **Very low efficiency** (~20–30%)
  * **High heat dissipation** (consumes power even without signal)

**Typical use:** audiophile amplifiers, preamplifiers, studio amplifiers.

### Class B

* **Principle:**
  Two transistors share the work
  one conducts the **positive half-cycle**, the other the **negative half-cycle**.

* **Advantages:**

  * **Higher efficiency** (~70%)
  * Less heat generation

* **Disadvantages:**

  * **Crossover distortion** occurs when switching between transistors
  * Lower fidelity compared to Class A

**Typical use:** systems prioritizing efficiency over precision.

### Class AB

* **Principle:**
  A combination of **Class A** and **Class B** designs.
  Each transistor conducts slightly more than half of the signal period, reducing crossover distortion.

* **Advantages:**

  * Good **balance between linearity and efficiency** (≈40–60%)
  * Low distortion

* **Disadvantages:**

  * Efficiency lower than Class B
  * Slightly more complex circuit design

**Typical use:** consumer audio, sound reinforcement, car amplifiers.

### Class C

* **Principle:**
  The transistor conducts for **less than half of the signal cycle**.

* **Advantages:**

  * **Very high efficiency** (up to 90%)

* **Disadvantages:**

  * **Extremely high distortion** — unsuitable for audio

**Typical use:** **RF circuits**, **oscillators**, and **transmitters**, where the output is later filtered.

### Class D (Switching / Digital Amplifiers)

* **Principle:**
  The input signal is converted into a **PWM (Pulse-Width Modulated)** waveform.
  The amplified pulses are then **filtered** to reconstruct the analog signal.

* **Advantages:**

  * **Excellent efficiency** (90–95%)
  * Compact and lightweight
  * Low heat generation

* **Disadvantages:**

  * **Switching noise** and possible **distortion**
  * Requires careful **output filtering**

**Typical use:** Bluetooth speakers, car radios, portable amplifiers, home theaters.

### Class E

* **Principle:**
  A variant of switching amplifiers optimized for **RF power transmission**.

* **Advantages:**

  * **Very high efficiency** (≈85–90%)
  * Suitable for **high-frequency applications**

* **Disadvantages:**

  * Strongly **nonlinear** → not suitable for audio

**Typical use:** RF transmitters, high-frequency power stages.

### Comparative Summary

| Class  | Type            | Efficiency | Distortion Level     | Primary Application      |
| :----- | :-------------- | :--------- | :------------------- | :----------------------- |
| **A**  | Linear          | 20–30%     | Very low             | High-end audio (Hi-Fi)   |
| **B**  | Linear          | ~70%       | Moderate (crossover) | Legacy audio, power amps |
| **AB** | Linear          | 40–60%     | Low                  | General-purpose audio    |
| **C**  | Nonlinear       | 80–90%     | Very high            | RF transmitters          |
| **D**  | Switching (PWM) | 90–95%     | Moderate–low         | Modern audio, portable   |
| **E**  | RF switching    | 85–90%     | Very high            | RF and microwave amps    |
