[![GenBio AI](https://raw.githubusercontent.com/genbio-ai/ModelGenerator/main/docs/docs/assets/images/genbio_header.png)](https://genbio.ai/)

# Research Overview

An AI-Driven Digital Organism (AIDO) is a system of integrated multiscale foundation models for predicting, simulating and programming biology at all levels. It is constructed in a modular, connectable, and holistic fashion to reflect biological scales, connectedness, and complexities. 

It is our view that a foundation model for biology — which can be a system of component FMs — needs to incorporate multiple types of data and biological constraints arising from different biological scales. Furthermore, such a system is more than just an agglomeration of modality-specific FMs. It must involve system-wide harmonization through nested or hierarchical representation propagation, utilization, fine-tuning, or continual pretraining. It should also have the ability to connect different FM modules from the system, and provide a foundation to address more complex prediction, simulation, and reprogramming tasks arising from molecules, cells, organisms, and beyond. 

Overall, our AIDO system consists of 4 layers: data layer, foundation model layer, downstream utility
layer, and applications of various types of bioengineering problems, as illustrated below:

![multiscalefm](https://github.com/user-attachments/assets/8b74e55b-ff2a-499e-9230-277317008011)

We took an engineering viable approach to building the AIDO in 3 stages. The first stage is to build up a necessary set of fundamental building blocks or modules representing the major data modalities arising in biology in a “divide-and-conquer” fashion. The second stage is to develop a set of new deep learning architectures that integrate the central dogma, regulatory rules, and the interconnected nature of biology, as well as different data modalities or modules in a bottom-up fashion to reflect the multiscale, nested, and hierarchical organization of biological systems. These architectures can bridge the existing gaps by integrating biological knowledge into the models and developing models that can seamlessly operate across various biological scales and modalities — thereby “dots are connected”. In the third stage, the modules and connected modules are unified into a networked system, where representations and embeddings can be passed around in different nodes and levels of the systems, and especially feedback and gradient signals from the coarser and topper level of the system can be propagated all the way back to the bottom level of the system to further improve these modules. This is like the “aligning and optimization” phase in an assembly process. With a set of benchmarks and supervisory tasks from different levels and scales of biology, all the system modules can be jointly adapted and aligned to achieve synergy towards an overall better or even emergent system-level performance.

As our initial release of the stage 1 of AIDO, we have completed the pretraining of the following set of foundation models: 
* AIDO.DNA --> GB.DNA
* AIDO.RNA --> GB.RNA
* AIDO.Protein --> GB.Protein
* AIDO.StructureTokenizer --> GB.StructureTokenizer
* AIDO.Cell --> GB.Cell
  
These pretrained foundation models and the correpsonding downstream utility layer for adapting these models and generating downstream task models are currently released as the AIDO.ModelGenerator repository:

[GB.ModelGenerator](https://github.com/genbio-ai/ModelGenerator)

and Hugging Face model checkpoints: 

https://huggingface.co/genbio-ai

Realizing the AIDO vision requires long-term, continuous, and sustainable development and commu-
nity efforts. In fostering such an effort, we shall make the weights of certain matured version of the
models and the adaptation software packages publicly available for reproducibility, community build-
ing, and standardization. The goal is to connect life science, medicine, pharmacy, and public health
through a shared technical paradigm, with a wider community involvement including academia, in-
dustries and governments, aligned on purpose-driven and coordinated massive data generation and
collection efforts, and close-loop collaboration on the full cycle of data, model, hypothesis, outcome,
back to more-data generation.

Through continuous versioning and upgrade of the base models, APIs, task-suites, data banks,
and bio-entity representation repositories, fueled by the ever-increasing willingness of data sharing and
federated data mining, and the never-fading demand for synthetic biology and personalized medicine,
we believe a new community of users and developers of an AIDO can emerge and grow from this open-
source effort as we have seen in the LLM field, to together pursue the common vision of mirroring life
in the physical world on a computer with AI. 

For more information on how to build an AI-Driven Digital Organism (AIDO), please also refer to this position paper: 

Le Song, Eran Segal, and E. P. Xing, Toward AI-Driven Digital Organism: Multiscale Foundation Models for Predicting, Simulating, and Programming Biology at All Levels, A position paper, [arXiv:2412.06993](https://arxiv.org/pdf/2412.06993), 2024.
