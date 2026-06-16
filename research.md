---
layout: page
title: Research
subtitle: Quantitative cell biology & non-equilibrium physics
permalink: /research/
---

I am interested in how living systems use energy to build and maintain order.
In the [Foster Lab](https://www.fosterlab.science/) at USC, I work on reconstituted
**kinesin–microtubule** systems — minimal active materials that let us measure, directly,
how molecular motors convert ATP into large-scale structural organization.

---

## Energy Dissipation & Self-Organization in Kinesin–Microtubule Active Networks
*Lead undergraduate researcher · Foster Lab · April 2025 – present*

How do ATP-driven molecular motors generate emergent structural order in active
microtubule networks? This project tries to connect the **molecular-scale energy
consumption** of motors to the **mesoscale organization** of the networks they build.

- **Built a new experimental system from scratch.** I independently developed the
  *maize kinesin-14* construct — sequence design, plasmid construction, cloning
  optimization, sequence verification, and bacmid generation for insect-cell expression.
- **Protein production.** Completed bacmid preparation and initiated insect-cell
  expression of mCherry-tagged maize kinesin-14 — one of five phylogenetically diverse
  kinesin-14 homologs in a comparative study.
- **Biophysical characterization (in progress).** ATPase activity, microtubule-binding
  assays, active contraction assays, and motor-driven network reconstitution.
- **Quantitative imaging.** Reconstituted kinesin–microtubule systems in vitro and observed
  active contraction by spinning-disk confocal microscopy; integrating NADH-coupled
  fluorescence assays with LC-PolScope microscopy to relate motor energy dissipation to
  emergent microtubule alignment.

> **The question in one line:** *Does the rate at which a motor burns energy predict the
> order of the structure it produces?*

---

## Modeling Plus-End Accumulation & Traffic Jams of Kinesin Motors
*Course research project (QBIO 482) · stochastic modeling in Python*

A computational counterpart to the wet-lab work: a stochastic 1D-lattice model of kinesin
transport along a microtubule, capturing motor binding, stepping, steric exclusion, and
site-specific dissociation.

- Implemented the **Gillespie stochastic simulation algorithm (SSA)** in Python to study
  emergent traffic-jam formation under varying motor concentrations and end-release rates.
- Ran systematic parameter sweeps over motor concentration and plus-end dissociation rate,
  quantifying steady-state density profiles, jam length, motor flux, and plus-end occupancy.
- Found **plus-end dissociation kinetics** to be the dominant regulator of accumulation —
  slow end release produces system-wide transport bottlenecks.
- Identified a **non-monotonic** concentration–efficiency relationship: more motors can
  *reduce* cargo flux through crowding-induced jamming.
- Validated against experimental observations from Leduc et al. (*PNAS*, 2012), connecting
  stochastic transport dynamics to axonal-transport dysfunction in neurodegeneration.

---

## Methods & Techniques

**Molecular biology** — plasmid design & cloning, PCR, gel electrophoresis, bacterial and
bacmid transformation, bacmid purification, DNA/RNA purification, baculovirus expression,
protein purification.

**Imaging** — spinning-disk confocal microscopy, LC-PolScope microscopy, quantitative
image analysis.

**Computation** — Python (NumPy, pandas, Matplotlib, scikit-learn), stochastic simulation
(Gillespie/SSA), R, C++.

---

*Interested in collaborating or want to hear more? [Get in touch](mailto:shenaugu@usc.edu).*
