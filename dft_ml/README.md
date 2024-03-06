# Density Functional Theory and ML

## overview

Motivation is to learn more about ml/computational approaches to DFT calculations.

Initial intuition was: Can AlphaFold/ColabFold be used for DFT?  
Seems unlikely at first glance, noting the lack of publicly available work on this approach.
Need to find out exactly why it wouldn't work if the above hypothesis is incorrect and document my learnings.

Also, to try out open source implementations that have been published for other approaches.



## notes

- [Paper: Deep dive into machine learning density functional theory for materials science and chemistry](https://journals.aps.org/prmaterials/pdf/10.1103/PhysRevMaterials.6.040301)
    - **From the abstract**: We provide the theoretical background of both DFT and machine learning on a generally accessible level. This serves as the basis of our comprehensive review, including research articles up to December 2020 in chemistry and materials science that employ machine-learning techniques.

- [Paper: From DFT to machine learning: recent approaches to materials science–a review](https://iopscience.iop.org/article/10.1088/2515-7639/ab084b/pdf)
    - **From the abstract**: This review follows a logical sequence starting from density functional theory as the representative instance of electronic structure methods, to the subsequent high-throughput approach, used to generate large amounts of data. Ultimately, data-driven strategies which include data mining, screening, and machine learning techniques, employ the data generated. We show how these approaches to modern computational materials science are being used to uncover complexities and design novel materials with enhanced properties. Finally, we point to the present research problems, challenges, and potential future perspectives of this new exciting field.

- [Combining DFT and Machine Learning: Towards faster and more accurate ab-initio calculations | Stony Brook Univ. Presentation](https://www.stonybrook.edu/commcms/iacs/_pdf/Sebastian%20Dick%20Presentation.pdf)
    
    - Useful introduction PPT to the topic.

- [Nature Paper: Completing density functional theory by machine learning hidden messages from molecules](https://www.nature.com/articles/s41524-020-0310-0)
    - **From the abstract**: Kohn–Sham density functional theory (DFT) is the basis of modern computational approaches to electronic structures. Their accuracy heavily relies on the exchange-correlation energy functional, which encapsulates electron–electron interaction beyond the classical model. As its universal form remains undiscovered, approximated functionals constructed with heuristic approaches are used for practical studies. 

- [PySCF](https://pyscf.org/) is an open-source collection of electronic structure modules powered by Python. The package provides a simple, lightweight, and efficient platform for quantum chemistry calculations and methodology development. PySCF can be used to simulate the properties of molecules, crystals, and custom Hamiltonians using mean-field and post-mean-field methods.

    - [PySCF User Guide Notebook](https://github.com/nmardirossian/PySCF_Tutorial/blob/master/user_guide.ipynb)

    - [Arxiv: PySCF: The Python-based Simulations of Chemistry
Framework](https://arxiv.org/pdf/1701.08223.pdf)




## links

- [Paper: Pushing the frontiers of density functionals by solving the fractional electron problem](https://www.science.org/doi/10.1126/science.abj6511)
    - Improving DFT with deep learning. Kirkpatrick et al. developed a framework to train a deep neural network on accurate chemical data and fractional electron constraints (see the Perspective by Perdew). The resulting functional outperforms traditional functionals on thorough benchmarks for main-group atoms and molecules. The present work offers a solution to a long-standing critical problem in DFT and demonstrates the success of combining DFT with the modern machine-learning methodology.
    NOTE: Only abstract. Open Access version of this paper was not found. 

- [Github Code: Deepmind Research: Pushing the Frontiers of Density Functionals by Solving the Fractional Electron Problem](https://github.com/google-deepmind/deepmind-research/tree/master/density_functional_approximation_dm21)
    - This package provides a PySCF interface to the DM21 (DeepMind 21) family of exchange-correlation functionals described in the paper ["Pushing the Frontiers of Density Functionals by Solving the Fractional Electron Problem"](https://www.science.org/doi/10.1126/science.abj6511).

- [ArXiv - Grad DFT: a software library for machine learning enhanced density functional theory](https://arxiv.org/pdf/2309.15127.pdf)
    - Grad
DFT: a fully differentiable JAX-based DFT library, enabling quick prototyping and experimentation
with machine learning-enhanced exchange-correlation energy functionals.
- [Scientists doubt that DeepMind's AI is as good for fractional-charge systems as it seems](https://phys.org/news/2022-08-scientists-deepmind-ai-good-fractional-charge.html)
    - A team of researchers from Skoltech, Zelinsky Institute of Organic Chemistry, HSE University, Yandex, and Kyungpook National University show in their comment in Science that DeepMind AI's ability to generalize the behavior of such systems does not follow from the published results and requires revisiting.

- [How to identify distant structural homologues - dealing with pLDDT and PAE](https://ftp.ebi.ac.uk/pub/training/2023/Structural_bioinformatics_2023/Day_4/AlphaFold/AlphaFold%20tutorial%20-%20structure.pdf)
    - This training materials overview is designed to provide a concise introduction to the identification of homologues and the use of pLDDT and PAE metrics from AlphaFold. The content will cover the fundamental principles of homology detection, the interpretation of AlphaFold's pLDDT scores for structural confidence, and the evaluation of protein structure prediction accuracy through PAE metrics.
    - [accesed from EMBL's European Bioinformatics Institute: AlphaFold Database and ColabFold tutorial ](https://www.ebi.ac.uk/training/materials/structural-bioinformatics-materials/protein-structure-prediction-and-molecular-docking/alphafold-database-and-colabfold/)

- [Medium: How to Install ColabFold & Run AI Protein Folding Locally](https://ai.plainenglish.io/how-to-install-colabfold-run-ai-protein-folding-locally-9467b57b9d37)
    - Useful tutorial to setup local Colabfold protein folding development
