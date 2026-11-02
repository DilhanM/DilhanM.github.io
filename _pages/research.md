---
layout: page
permalink: /research/
title: Research
nav: true
nav_order: 2
---

<style>
  /* Layout for this page: justified text, figures at the top right with text wrapping around them,
     each section heading starting below the previous section's figure. Figures go full width on phones. */
  article p {
    text-align: justify;
  }
  article figure {
    float: right;
    width: 50%;
    margin: 0.3rem 0 1rem 1.5rem;
  }
  article figure .caption {
    text-align: left;
  }
  article h4 {
    clear: both;
  }
  @media (max-width: 576px) {
    article figure {
      float: none;
      width: 100%;
      margin: 0 0 1rem 0;
    }
  }
</style>

#### Quantum Molecular Structure Encoding

{% include figure.liquid path="assets/img/research/qmse-circuit.png" class="img-fluid rounded" caption="<b>Figure 1.</b> QMSE encoding of butanone. Top left: structural formula of butanone with numbered atoms. Top right: the data encoding matrix, where diagonal entries map to atomic masses and off-diagonal entries encode bonded atom pair masses and bond order. Bottom: the resulting parametrised quantum circuit, where diagonal and off-diagonal entries of the encoding matrix map to single- and two-qubit gates respectively." alt="Quantum molecular structure encoding of 2-butanone: numbered molecular structure, its hybrid-adjacency encoding matrix, and the corresponding quantum circuit of Ry and Rxx rotations" %}

Mapping a dataset onto a quantum circuit, known as data encoding, is the first step in any quantum machine learning (QML) algorithm. The choice of encoding determines how well a quantum learning model can distinguish between inputs. For chemical applications, it is therefore natural to look for bespoke encoding schemes that can capture the rich structural information in chemical data. We developed [Quantum Molecular Structure Encoding](https://doi.org/10.1088/2632-2153/ae304f) (QMSE), a chemically aware data encoding scheme that maps molecular structural properties to quantum circuits. Atomic masses and bond orders are mapped to single- and two-qubit rotations in a parametrised quantum circuit, as demonstrated for butanone in Figure 1. QMSE improves the state separability between encoded molecules compared to conventional QML data encoding schemes, and outperforms them on classification and regression benchmarks.

We are now extending QMSE beyond small organic molecules into a general-purpose chemical data encoding framework for QML, and applying it to a range of different chemical systems.

#### Quantum Algorithms for Electronic Structure

In collaboration with AstraZeneca, Algotithmiq, IBM, and the Hartree Centre, we demonstrated a quantum computing pipeline for [modelling proton-transfer processes](https://doi.org/10.1039/D5CP04097C) on quantum computers, treating both electrons and nuclei quantum mechanically. Starting from a highly accurate but resource-intensive setup, we showed how systematic approximations can be applied to construct quantum circuits that still capture the important physics of proton transfer.

More recently, hybrid quantum-classical algorithms based on the [Quantum Selected Configuration Interaction](https://doi.org/10.1103/dmn4-snfx) (QSCI) method have gained a lot of interest in the quantum computing community. These methods work by sampling a quantum state prepared on a quantum processor, and projecting the system Hamiltonian onto the subspace spanned by the configurations sampled by the quantum device. The projected Hamiltonian is then diagonalised classically. We are now exploring methods in this family, such as [SqDRIFT](https://arxiv.org/abs/2508.02578), for challenging electronic structure problems in chemistry.
