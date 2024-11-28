# Exploring π Through Collisions

This small project demonstrates how the mathematical constant π emerges from a fascinating physics experiment involving collisions between two masses and an immovable wall.

---

## The Setup
Imagine two objects with masses \(m_1\) and \(m_2\), along with an immovable wall. The masses move and collide with each other and the wall, obeying the laws of elastic collisions.

- **Masses**: \(m_1 = 1\), \(m_2 = 100^n\), where \(n \in \{0, 1, 2, \dots\}\)
- **Wall**: Positioned to the left of \(m_1\), preventing further motion.

---

## Key Insight: Collisions and π
The total number of collisions in this setup is directly related to the digits of π:

- If \(n = 0\), the number of collisions is **3** (first digit of π).
- If \(n = 1\), the number of collisions is **31** (first two digits of π).
- If \(n = 2\), the number of collisions is **314** (first three digits of π).
- And so on...

This remarkable result connects the physical behavior of the system to the digits of π!


# Buffon's Needle Problem

This project simulates **Buffon's Needle Problem**, a famous probability experiment used to estimate the value of π (pi) through random sampling. The problem was posed by Georges-Louis Leclerc, Comte de Buffon, in the 18th century and is one of the earliest examples of a Monte Carlo simulation.

---

##  Problem Statement

Imagine a floor with evenly spaced parallel lines, separated by a distance \(d\). A needle of length \(L\) (\(L \leq d\)) is randomly dropped onto the floor. The problem is to calculate the probability that the needle crosses one of the lines.

### Key Formula

The probability \(P\) is given by:
\[
P = \frac{2L}{\pi d}
\]

From this, we can estimate the value of \(\pi\) using:
\[
\pi \approx \frac{2L \times N}{d \times C}
\]
where:
- \(N\): Total number of needles dropped
- \(C\): Number of needles that cross a line

---

##  Project Overview

This Python project uses a **Monte Carlo simulation** to estimate the value of \(\pi\). By dropping a large number of virtual needles onto a floor and calculating how many cross the lines, we approximate \(\pi\).

### Steps:
1. Randomly generate the position and angle of a needle.
2. Check if the needle crosses a line.
3. Repeat for a large number of needles.
4. Use the formula above to calculate \(\pi\).
