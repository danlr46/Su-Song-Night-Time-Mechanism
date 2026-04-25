# Su-Song-Night-Time-Mechanism
Proposed reconstruction of the night-time time-signaling system of Su Song’s water-driven astronomical clock tower (11th century).
Su Song Night-Time Mechanism Reconstruction

This repository presents a proposed mechanical reconstruction of the night-time time-signaling system of Su Song’s water-driven astronomical clock tower (11th century), based on textual analysis of the Xin Yi Xiang Fa Yao and on kinematic modeling.

⸻

Overview

Su Song’s clock tower combined astronomical observation and timekeeping within a single integrated system.
While the daytime subsystem measured mean solar time, the night-time subsystem had to regulate a sequence of signals (gōng and drum strikes) according to the changing duration of the night across the seasons.

The original text describes the use of sixty-one arrows, replaced periodically, but does not explain the mechanical implementation.
This work proposes a reconstruction based on two coupled mechanisms:

* a phase-control system, adjusted discretely through the insertion of arrows
* a fan-like redistribution system, which repositions the wooden figures according to night duration

Together, these mechanisms allow the system to synchronize a sequence of acoustic signals with a seasonally varying night, without the need for continuous annual gearing.

⸻

Repository Contents

1. Night watch Su Song

Computes the geometry of the phase-control cam (arrow wheel), based on astronomical data for Kaifeng.

Main functions:

* computation of solar declination and day length
* derivation of sunset variation over the year
* inverse kinematics to obtain the cam profile
* discretization into 61 positions (six-day intervals)

⸻

2. WoodenFiguresFanMechanism.ipynb

Simulates the fan-like mechanism governing the wooden figures on the fifth level.

Main features:

* 31 ribs rotating around a central pivot
* spiral cam slots generating radial displacement
* symmetric expansion/contraction of the fan
* mapping between phase control and spatial redistribution

⸻

3. NightTime FullAnimation.ipynb

Generates a full animation of the system, including:

* phase-control mechanism (fourth level)
* fan mechanism (fifth level)
* transmission through a vertical shaft
* four-gear kinematic chain
* axonometric projection of the complete system

⸻

Proposed Mechanical Solution

The reconstruction is based on the following principles:

1. Discrete phase control
    The sixty-one arrows described by Su Song are interpreted as discrete inputs, replaced approximately every six days according to the solar terms.
    Each arrow sets the angular position of a gear, thereby defining the phase of the system.
2. Unit transmission chain
    A system of four gears (15:30 and 30:15 ratios) transmits the angular displacement without amplification or inversion, preserving both magnitude and direction.
3. Fan-like redistribution of wooden figures
    The wooden figures are mounted on ribs forming a fan structure.
    A cam-driven mechanism adjusts their angular distribution between approximately 145° and 215°, reflecting the seasonal variation in night duration.
4. Direct triggering through trip-teeth (撥牙, bō yá)
    Each figure carries a trip-tooth that activates the gong or drum when reaching a specific angular position, eliminating the need for a separate trigger lever.

This configuration allows the system to regulate night-time signals through discrete adjustments rather than continuous modulation.

⸻

Conceptual Framework

Unlike later Western clocks, which solved seasonal irregularities through continuous cam-based mechanisms, this reconstruction suggests a different approach:

* continuous motion for the driving system
* discrete adjustment for seasonal synchronization
* human intervention as part of the control loop

In this sense, the system operates as a form of mechanical programming based on periodic updates.

⸻

Requirements

* Python 3.x
* NumPy
* Matplotlib
* Jupyter Notebook

⸻

Output

The repository produces:

* cam profiles for the phase-control mechanism
* simulation of the fan mechanism
* full animated visualization of the system

⸻

Notes

This reconstruction is hypothetical and intended as a kinematic and conceptual model consistent with the available textual evidence.
It does not claim to represent the exact historical mechanism, but rather a plausible solution compatible with the descriptions provided by Su Song.

⸻

Author

Daniele L. R. Marini
