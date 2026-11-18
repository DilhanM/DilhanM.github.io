---
layout: page
title: People
permalink: /people/
nav: true
nav_order: 1.5 # between About and Research (2)
---

<style>
  /* Justified text, photos at the top right with text wrapping around them. Photos go full width on phones. */
  article p {
    text-align: justify;
  }
  article figure {
    float: right;
    width: 30%;
    margin: 0.3rem 0 1rem 1.5rem;
  }
  article h4 {
    clear: both;
  }
  /* Keep the last photo from spilling past the end of the page. */
  article::after {
    content: "";
    display: block;
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

#### Dr Dilhan Manawadu

{% include figure.liquid path="assets/img/prof_pic.jpg" class="img-fluid rounded z-depth-1" alt="Dilhan Manawadu" %}

Dilhan is a quantum computational chemist at the University of Liverpool. Originally from Sri Lanka, he obtained his BSc, specialising in Chemistry, from the University of Colombo. He joined the University of Oxford in 2018, where he received an MSc in Theoretical and Computational Chemistry, followed by a DPhil investigating the photoexcitations of linear polyenes using Density Matrix Renormalisation Group (DMRG) techniques. He then joined the STFC Hartree Centre as a Quantum Software Engineer, working on a range of projects developing and deploying quantum computing algorithms for industry-relevant research problems in chemistry.

In September 2026, he joined the Department of Chemistry at the University of Liverpool as a tenure-track fellow.

#### Kajanann Karunaivel

{% include figure.liquid path="assets/img/kaj.jpeg" class="img-fluid rounded z-depth-1" alt="Kajanann Karunaivel" %}

Kaj is an MChem Medicinal Chemistry student who enjoys chemistry in all its aspects, with specific interests in synthetic, theoretical and applied chemistry, and further interests in quantum mechanics and organic chemistry. Kaj is currently investigating extensions of Quantum Molecular Structure Encoding to conjugated molecules, with the hope of making advances within the project and the wider research area.

His hobbies include watching movies, shows and anime, K-pop, the gym, martial arts, dancing, and just living life with fun!

Interested in joining the group? See [Join Us](/join/).
