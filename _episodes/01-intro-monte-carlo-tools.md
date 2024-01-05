---
title: "Introduction to LHC Event Generation Chain"
teaching: 30
exercises: 5
questions:
- "What are the monte carlo tools used to generate events at LHC?"
- "How do the tools differ from each other?"
objectives:
- "Learn about common monte carlo tools at the LHC"
- "Introduce the steps involved in LHC event generation"
keypoints:
-

---

Particle Physics collider experiments involve the study of scattering processes wherein two initial particles scatter into final particles leading to two or more particles in the final state. In the present times, the Large Hadron Collider at CERN is the largest particle collider and it consists of four experiments, namely, the  general purpose experiments viz. ATLAS and CMS, the LHCb which concerns the flavour physics studies, and the ALICE experiment which involves studies related to Heavy-ions. There are also other ongoing experiments such as the Belle2 experiment, and others. Moreover, future colliders such as the Future Circular Collider (ee, hh), International Linear Collider (ee), and Muon Colliders are also being planned.

The particle physicist working on the present and future collider experiments (in particular, the detector) often make use of "Monte Carlo Event Generators" to study the physics process of interest. A Monte Carlo Event Generator is a tool that makes use of the "Monte Carlo" technique to simulate a scattering process ('event').  In particular, the typical workflow involved in particle physics is as follows - Theorists design physics models that may be tested at the collider experiments; these physics models are then brought to a form such that they can be used computationally in Monte Carlo Event Generators. The model building stage can be achieved by using, for instance, FeynRules framework. The output of tools like FeynRules is often produced in a Universal Feynman Rules Output (UFO) files which are then shared by theorist/phenomenologist on HEP forums such as this one [LINK](http://feynrules.irmp.ucl.ac.be/wiki/ModelDatabaseMainPage).

The obtained UFO files are then used in a Monte Carlo Event Generator that generates the (parton level) matrix elements for the physics process (for example, MadGraph5_aMC@NLO, Whizard). These parton level events then undergo a parton shower in software such as Pythia8. The parton-showered files are then processed so as to apply fast/full detector simulation.  Monte Carlo tools forms the backbone of particle physics. These tools are not only useful in collider phenomenology, but also in the neutrino experiments.

However, Monte Carlo Event Generators are often used as blackboxes. Therefore, it is crucial to decipher the underlying physics and computational techniques that are used in the development of these tools, which will also lead to a better understanding of the limits of these tools. This tutorial is dedicated to understanding the main methods that are used by the Monte Carlo Event Generator as well as learning some of the well-know event generators like the MadGraph5_aMC@NLO, Pythia8 and Whizard3.

As optional studies, one will also learn some basics of Generative Adversarial Neural Network to generate Monte Carlo Samples.
