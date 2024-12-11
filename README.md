
```davidnovak9000 at gmail dot com```

### [Full CV available here.](cv.pdf)

I am a bioinformatician and PhD researcher at [Saeys lab](https://saeyslab.sites.vib.be/en), [Center for Inflammation Research](https://www.irc.ugent.be) of the Flemish Institute of Biotechnology and Ghent University in Ghent, Belgium, working on an [FWO Strategic Basic research](https://www.fwo.be/en/fellowships-funding/phd-fellowships/phd-fellowship-strategic-basic-research/) project.
Before that, I worked at [Childhood Leukaemia Investigation Prague (CLIP)](https://clip.lf2.cuni.cz/en) in Czechia.

I make robust and interpretable machine learning and statistical models for single-cell data analysis.

#### **I am open to work (and relocation) from Q2 of 2025.**

See my [Google Scholar](https://scholar.google.com/citations?user=FU7FJPcAAAAJ&hl=en) profile for publication activity.

Some of my public project repositories, including collaborations, are listed below.

## Dimensionality reduction and structure learning

### [**ViVAE**](https://github.com/saeyslab/ViVAE)

*ViVAE* is an embedding framework that demonstrably improves structure preservation, interpretability and QC in scRNA-seq dimensionality reduction.
Using VAEs, a novel stochastic-MDS loss (based on [SQuadMDS](https://github.com/PierreLambert3/SQuaD-MDS-and-FItSNE-hybrid)) and data de-noising, we achieve a better balance of local and global structure preservation with scRNA-seq data.
Additionally, the model is equipped with a novel and generalisable algorithm for detecting latent space distortions (encoder indicatrices) and integrates with [FlowSOM](https://github.com/saeyslab/FlowSOM_Python).
I am the first author the associated manuscript, penned with my co-authors from Ghent University and UCLouvain (read current [pre-print](https://www.biorxiv.org/content/10.1101/2023.11.23.568428v3) here).
The work was presented at CYTO 2024.

### [**GroupEnc**](https://github.com/saeyslab/GroupEnc)

*GroupEnc* is a proof-of-concept project for parametric multi-dimensional scaling (MDS) on GPU, presented at BNAIC/BeNeLearn 2023.

## Differential expression testing

### **Large-scale cytometry differential testing pipeline for large cohorts**
*A public repository with a novel pipeline for robust differential expression modelling in large flow cytometry data cohorts will soon be added.*

### [**tidycell**](https://github.com/davnovak/tidycell)

*tidycell* is a basic differential expression analysis tool written in R for cytometry data.
I developed during my time at [Childhood Leukaemia Investigation Prague](https://clip.lf2.cuni.cz/cs).
It has been applied on GvHD data and in a project on head & neck cancers at [Biocev](https://www.biocev.eu/en).

## Topological trajectory inference

### [**tviblindi**](https://github.com/stuchly/tviblindi)

*tviblindi* is a semi-supervised single-cell TI tool that uses TDA and persistent homology to work with high-dimensional data.
For my master thesis, I implemented parts of the TDA pipeline in C++ and created a method for clustering trajectories based on persistent homology, as well a GUI in Shiny.
The tool has since been applied successfully to create multi-organ models of development that refine descriptions of human [B-cell](https://onlinelibrary.wiley.com/doi/10.1002/eji.202451004) and [T-cell](https://elifesciences.org/reviewed-preprints/95861/figures) development.

## (Semi-)automated single-cell data annotation

### [**hloss**](https://github.com/davnovak/hloss)

*hloss* is a work I presented at the ABLS 2022 bioinformatics conference.
It tackles the issue of evaluating cell type classification in single-cell data in a way that reflects known hierarchies and ontologies.
A novel scoring approach incorporates a biological prior to assess error based on degrees of relatedness.

### [**SplitScore**](https://github.com/davnovak/SplitScore)

Work in progress on alternatives to hierarchical metaclustering done by [FlowSOM](https://github.com/saeyslab/FlowSOM).
Clusters are merged so as to preserve reasonable signal distributions per channel.
In practice, this can be done through preserving unimodality of marker expression (for cytometry data).
This is an ongoing effort, since the requirement of preserving some distribution modalities in metaclustering arises now and then in different projects.

## Evaluation and benchmarking

### [**ViScore**](https://github.com/saeyslab/ViScore)

*ViScore* is a collection of evaluation metrics for dimensionality reduction that address past problems with fairness and scalability.
Together with collaborators from UCLouvain, we have released a battery of both unsupervised and supervised evaluation algorithms and an extensible HPC benchmarking framework.
We build on the RNX curves and the [Neighbouhood Proportion Error](https://github.com/akonstodata/NPE) to provide novel embedding-level and population-level scores.
This is described in our *ViVAE* [pre-print](https://www.biorxiv.org/content/10.1101/2023.11.23.568428v3).

### [**SingleBench**](https://github.com/davnovak/SingleBench)

*SingleBench* is a benchmarking framework for high-dimensional data transformations and clustering in R.
Relying on HDF5 and recycling of intermediate results, it enables extensive hyperparameter sweep and easy interpretation of results.
I presented this work at CYTO 2021.
I recently picked this project up again: more results to come.

## Cytometry utilities

### [**qctoy**](https://github.com/davnovak/qctoy)

*qctoy* is an R package for simulating aberrances in flow cytometry measurements that are relevant in designing QC tools and pipelines.
I developed this small tool during a summer internship at SaeysLab to help with designing the QC algorithm what eventually became [PeacoQC](https://bioconductor.org/packages/release/bioc/html/PeacoQC.html).

### [**auto_compensate**](https://github.com/davnovak/auto_compensate)

*auto_compensate* is an automated pipeline for cytometry data compensation I designed for [Childhood Leukaemia Investigation Prague](https://clip.lf2.cuni.cz/cs).

## Miscellaneous

### [**hidden**](https://github.com/davnovak/hidden)

*hidden* is a hidden Markov model simulator in R.
I wrote it to understand HMMs better.

### [**CommandLineParser**](https://github.com/katebrich/command_line_parser)

*CommandLineParser* is a C#/.NET API I co-wrote with [Kačka Břicháčková](https://github.com/katebrich).
This is a course project we teamed up for during our Master's in Bioinformatics at Charles University.

### [**avl_tree**](https://github.com/davnovak/avl_tree)

*avl_tree* is an Adelson-Velsky and Landis tree implementation in Pascal.
It's some of my earliest code, written during my Bachelor's in Biology during which I took elective comp sci courses.

### [**RCondaRun**](https://github.com/davnovak/RCondaRun)

*RCondaRun* is a tiny package for switching between Conda environments within a single R session when interfacing with Python.

<hr>

Interested in my work or collaborating?
Feel free to reach out.

![portrait](./portrait.png)
