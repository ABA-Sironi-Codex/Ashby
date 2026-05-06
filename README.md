# Ashby

## A pseudo-organic digital homeostat

**Live Demo:** [https://davideriboli.github.io/Ashby/](<https://davideriboli.github.io/Ashby/> "null")

> "The Homeostat is the first machine to be built with a goal-seeking mechanism, not by design, but by chance." — W. Ross Ashby

### Overview

**Ashby** is a generative art piece and cybernetic simulation inspired by William Ross Ashby’s 1948 "Homeostat." This project translates the pioneering concepts of *ultrastability* and *homeostasis* into a pseudo-organic digital ecosystem.

In this simulation, four interconnected "cells" attempt to maintain internal stability (equilibrium) while being constantly perturbed by an unpredictable environment.

### What is a Homeostat?

The original Homeostat was an electromechanical device built by British psychiatrist and cyberneticist W. Ross Ashby. It was designed to demonstrate how a machine could achieve stability through adaptation without having a pre-programmed solution.

<img width="960" height="779" alt="960px-W _Ross_Ashby&#39;s_1948_Homeostat" src="https://github.com/user-attachments/assets/dfe8d862-8d12-4eb8-8528-45b4e02695f0" />

*The original homeostat, built in 1948 by W. Ross Ashby*.

**Core Principles:**

1. **Essential Variables:** Every organism has variables (like body temperature) that must stay within specific limits to ensure survival.

2. **Ultrastability:** When a variable exceeds its critical threshold, the system is no longer stable. Instead of failing, the Homeostat randomly reorganizes its internal connections (synapses) until it finds a new configuration that restores equilibrium.

3. **Feedback Loops:** The system is in constant dialogue with the environment, reacting to disturbances through a complex matrix of weighted connections.

### Technical Implementation

This digital interpretation utilizes **HTML5 Canvas** and **Vanilla JavaScript** to simulate the cybernetic matrix.

- **Biological Aesthetic:** The four units of the original machine are represented as biological cells floating in a "primordial soup."

- **The Matrix:** The system is governed by a 4x4 weight matrix ($dV/dt = W \cdot V$). Each cell’s state influences the others.

- **The Step-Switch Mechanism:** When a cell's stress (essential variable) hits the **Critical Threshold**, the system triggers a "Chaos" event, mimicking Ashby's uniselectors. It randomizes the weights in the matrix until the cells stop oscillating.

- **Real-time Monitoring:** The dashboard calculates the **Recovery Time**, tracking exactly how long the system takes to find a new stable configuration after a disturbance.

### Controls

- **Interaction:** Click or drag your cursor across the background to "inject" environmental stress.

- **Critical Threshold:** Adjust how much stress a cell can handle before triggering a mutation.

- **Natural Recovery:** Adjust the innate "cooling" or damping effect of the organism.

- **Environmental Sensitivity:** Change how violently the cells react to your mouse movements.

- **Force Chaos:** Manually trigger a structural reorganization (formerly "Force Mutation").

- **Force Homeostasis:** Artificially guide the system back to a near-stable state to observe the final stages of recovery.

### Development

Built with a focus on clean, high-contrast UI and fluid animation:

- **Language:** HTML5, CSS3, JavaScript (ES6+).

- **Mathematics:** Matrix-based differential interaction and debounce logic for stability verification.

*Created as an exploration of early AI history and generative biological systems.*

