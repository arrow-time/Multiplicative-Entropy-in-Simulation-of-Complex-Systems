# Multiplicative Entropy in Simulation of Complex Systems

Zou, Zhi Kai
Independent Researcher; Shenzhen; China; zhiyan.zou@foxmail.com

Abstract: Multiplicative entropy is a non-statistical, computable, high-resolution, algebraic form of entropy developed by the author since February 2025[1] in related thermodynamics time theory. By multiplying the values of each unit in a system, multiplicative entropy provides a simple, real-time computable, path-recordable evolution indicator for complex system simulation, allowing researchers to intuitively track the entire process from initial state to distribution homogenization of system value. This brief report primarily adapts and supplements the applicable conditions for complex system applications, while introducing the potential of multiplicative entropy in this field. 

A system can adopt a multiplicative entropy description if it satisfies the following conditions:

##### 1.The number of units carrying numerical values remains constant.

##### 2.Each unit is associated with a quantifiable value (e.g., energy, resource amount, or population size).

##### 3.The total sum of all unit values is conserved.

##### 4.The dynamical evolution follows a flow or exchange rule wherein quantities transfer from units with higher values to those with lower values.

##### 5. The numerical value carried by each unit must be unitized, i.e., expressed as an integer multiple greater than 1 of the basic unit.

Keywords: multiplicative entropy; complex system entropy coordinate; complex system evolution path analysis; computable entropy; non-statistical entropy; high-resolution entropy; algebraic entropy; analytic entropy; 

Introduction: In the study of complex systems, we often face a challenge: the system is constantly changing internally, yet we lack an indicator that can clearly depict the "process of change." Taking an ecosystem as an example, we know that it will eventually tend toward some equilibrium, and we also know that species distribution is relatively uniform at equilibrium. However, it is difficult to describe "how the system state evolves at each step from the beginning to equilibrium." Traditional entropy can tell us the difference between the starting point and the endpoint, but the intermediate process is a black box. Multiplicative entropy provides a way to make the process of entropy increase more visible.

What is Multiplicative Entropy?
The definition of multiplicative entropy is straightforward: If a system has a constant number of units that carry energy (or some numerical value) (which can also be understood as a fixed coarse-graining level of a discrete system), the total energy of the system (total numerical value, hereafter using energy as an example) is conserved—meaning the sum of energies carried by all units is constant—and the energy transfer rule of the system is that energy conducts from high to low between adjacent units, then the entropy value of the system is obtained by multiplying the energy values (or other value) of each unit in this system. The constant energy sum corresponds to the First Law of Thermodynamics: energy conservation; the monotonic increase of the cumulative product corresponds to the Second Law of Thermodynamics, the law of entropy increase. Under these conditions, the cumulative product of the numerical values carried by the value-carrying units within the system increases monotonically and has an upper limit, consistent with the traditional thermodynamic definition of entropy for a closed system. For detailed proof processes, please refer to several works by the author since May 2025 [2].

The entropy value of a closed system at a given moment: S = ∏mᵢ; i∈N  ①
The sum of numerical values in a closed system = constant = ∑mᵢ; i∈N  ②
mᵢ refers to the numerical value carried by the i-th system unit.

A simple example is provided below:
Suppose a simple system consists of four units, and their energies are [3, 1, 5, 3] respectively. Then the multiplicative entropy at this moment is:
The energy sum of this system is 3+1+5+3=12
The entropy of the initial state is 3 × 1 × 5 × 3 = 45
If the system undergoes one energy transfer to the next state—for instance, one unit transfers 1 unit of energy to another unit—the energy distribution becomes [3, 1, 4, 4], and the new entropy is:
3 × 1 × 4 × 4 = 48
With each update of the system's numerical distribution, the entropy value increases monotonically, and the total system value remains unchanged throughout the process.

How is it Different from Traditional Entropy?
Entropy in traditional thermodynamics (such as Boltzmann entropy) is a state function. It tells us "what state the system is in now" and "where it will eventually go," but it rarely addresses "what happened in between."

Multiplicative entropy, in contrast, is a non-statistical path function. It allows us to record the entropy value at each step during the system's evolution, thereby obtaining a complete "entropy evolution trajectory" that can serve as a high-resolution thermodynamic coordinate for the system's evolution.

For example, consider a system starting from [3,1,5,3] and eventually reaching the uniform state [3,3,3,3]. Different evolutionary paths produce different intermediate entropy value sequences:

Path A: [3,1,5,3] → [3,1,4,4] → [3,2,3,4] → [3,3,3,3]
Entropy values: 45 → 48 → 72 → 81

Path B: [3,1,5,3] → [3,2,4,3] → [3,3,3,3]
Entropy values: 45 → 72 → 81

Both paths ultimately reach the same final steady state, but the intermediate entropy change processes are completely different. Multiplicative entropy enables us to distinguish between them.


Why is this useful for complex system simulation?
One of the core characteristics of complex systems is the irreversibility of processes and the diversity of paths. Whether it is the energy distribution in climate systems, the flow changes in traffic networks, or the movement of resources in economic systems, we are often concerned not only with "whether equilibrium is ultimately reached" but also with "how it reaches equilibrium"—for instance, whether there are critical points, fluctuations, or stagnation points during the process.

Multiplicative entropy provides a feasible technical tool for this type of research:
Real-time computable: In computer simulations, each time the system state is updated, the new multiplicative entropy can be immediately calculated.
Path-recordable: The entropy changes throughout the entire evolution process can be saved, forming an "entropy curve" for analyzing the system's dynamic characteristics.
Comparable across different paths: For the same starting point and endpoint, different evolution mechanisms produce different entropy curves, providing a quantitative basis for comparing and optimizing system evolution paths.

Its Applicable Conditions
Multiplicative entropy is not a one-size-fits-all solution. It is suitable for systems that meet the following conditions:
The number of units carrying numerical values in the system remains constant.
Each unit has a quantifiable numerical value (such as energy, resource quantity, population size, etc.).
The total sum of numerical values in the system is conserved (the sum of all unit values is fixed).
Evolution rule: Flow or exchange exists between units, and the direction of flow is from high-value units to low-value units.
The numerical value carried by each unit must be unitized, i.e., expressed as an integer multiple greater than 1 of the basic unit.

Under these conditions, multiplicative entropy increases monotonically as the system's numerical values evolve toward a uniform distribution. This monotonicity is not assumed but is a mathematical necessity: as long as values flow from high places to low places, the product increases.

A Simple Simulation Approach
If attempting to use multiplicative entropy in research on a system that meets the applicable conditions, the simulation can be designed as follows:

1.Initialize a system composed of N units, assigning initial numerical values to each unit (ensuring the sum is constant).
2.Define the connection relationships between units and the rules for value flow.
3.Run the simulation, calculating the new multiplicative entropy after each energy exchange (each update of the system's energy distribution state).
4.Record the entropy value at each step and plot the entropy change curve.
5.Compare entropy curves under different parameter settings to analyze the system's evolution characteristics.

This type of simulation does not require complex mathematical derivations; it only needs basic arithmetic operations and recording functions. However, it can provide a "process perspective" that traditional entropy cannot offer.

Discussion
Multiplicative entropy is not a concept intended to replace traditional entropy, but rather a complement. Its value lies in enabling researchers to "see" the intermediate processes of system evolution, rather than only the starting point and endpoint.
For complex systems research, this focus on process may be precisely what we need. After all, in many practical problems—such as climate change, ecological protection, and economic regulation—we want to know not only "what will ultimately happen to the system," but also the specific process of evolution. By comparing entropy change curves under different evolution paths, the system's homogenization rate, path dependence, and critical behavior can be quantitatively analyzed.
Multiplicative entropy offers a way to address this question using simple arithmetic.
This provides only a brief introduction to multiplicative entropy for researchers in complex systems; specific applications can be developed by professional complex systems experts.
We welcome guidance and collaboration.

[1 ]original manuscript since February 2025 :https://doi.org/10.5281/zenodo.14788393

[2] Zou, Z. K. (2025). Time-Entropy Mirroring via Space Transformation and Mass-Gravity Duality via QCD-Higgs Synergy. Preprints. https://doi.org/10.20944/preprints202505.0270.v1
