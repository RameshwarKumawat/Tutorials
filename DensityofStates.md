# Density of States (DOS) Theory

## 1. Introduction

The **Density of States (DOS)**, denoted as $g(E)$, describes the number of electronic states available at each energy level per unit volume and per unit energy.

It's essential for:
- Determining **carrier concentrations**
- Modeling **transport** and **optical** behavior in semiconductors
- Understanding the behavior of **quantum materials** (e.g., 2D materials, nanostructures)

---

## 2. General Definition

The DOS is defined as:

$$
g(E) = \frac{dN}{dE}
$$

Where:
- $g(E)$: Number of available states per unit energy
- $N(E)$: Total number of states below energy $E$

For free electrons in a crystal:

$$
E = \frac{\hbar^2 k^2}{2m^*}
$$

---

## 3. DOS in Different Dimensions

### 3.1 One-Dimensional (1D)

For a quantum wire:

$$
g_{1D}(E) = \frac{1}{\pi} \cdot \frac{1}{\hbar} \cdot \sqrt{\frac{m^*}{2(E - E_c)}}
$$

- Diverges at the conduction band edge ($E = E_c$)
- Shows van Hove singularity

---

### 3.2 Two-Dimensional (2D)

For a quantum well or 2D electron gas:

$$
g_{2D}(E) = \frac{m^*}{\pi \hbar^2}
$$

- **Constant** with energy above each subband
- Causes **step-like** increases in total DOS as new subbands become available

---

### 3.3 Three-Dimensional (3D)

For bulk semiconductors:

$$
g_{3D}(E) = \frac{1}{2\pi^2} \left( \frac{2m^*}{\hbar^2} \right)^{3/2} \sqrt{E - E_c}
$$

- Increases as $\sqrt{E - E_c}$
- Smooth behavior near the band edge

---

## 4. Physical Interpretation

DOS represents the number of available quantum states for electrons to occupy at a specific energy.

To find the carrier concentration in the conduction band:

$$
n = \int_{E_c}^{\infty} g(E) f(E) \, dE
$$

Where:
- $f(E)$: Fermi-Dirac distribution function

---

## 5. DOS Schematic Diagram

    DOS g(E)
      ↑
      |
      |───────┐                      (2D)
      |       │
      |       │
      |       │        .            (3D)
      |       │       .
      |       │     .
      |       │   .
      |       │.                      (1D)
      |       └─────────────────────────────→ E
             ↑
        Conduction
         Band Edge
