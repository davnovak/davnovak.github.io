
```davidnovak9000 at gmail dot com```

[CV](cv.pdf) • [Google Scholar page](https://scholar.google.com/citations?user=FU7FJPcAAAAJ&hl=en) • [GitHub page](https://github.com/davnovak)

Hi there! I'm a *bioinformatician/computational biologist* and PhD researcher at [Saeys lab](https://saeyslab.sites.vib.be/en), Flemish Institute of Biotechnology in Belgium.
The focus of my PhD has been exploratory and statistical modelling of **high-dimensional cytometry** and **single-cell RNA-seq data**.
I love collaborating with immunologists, bioinformaticians and computer scientists alike, and **delivering interpretable and interactive solutions to all the problems involved with big and complex data**.
That includes effective presentation of results, complex data visualisation and designing graphical user interfaces to empower domain experts.

I enjoy teaching and tutoring, having co-taught **machine learning** at Ghent University for 4 years, which involved **guiding over 200 students** through practicals and helping them design and carry out semestral projects.
I also co-organised the successful [Computational Cytometry Summer School 2024](https://training.vib.be/all-trainings/computational-cytometry-summer-school) where I taught statistical analyses of cytometry data.

I'm proficient in **R & Python** for data analysis and deeply familiar with **high-dimensional cytometry and scRNA-seq data**, having built and maintained large analytical pipelines, and written new algorithms to advance the state-of-the-art in interpretable single-cell analysis.
Other IT-related skills are listed in my [CV](cv.pdf).

<details>
<summary><b>My background</b></summary>
<br>

A biology undergrad, I shifted toward bioinformatics a year into my studies, and went on to do a Master's and PhD in it (which I'm finishing up now).

My research started out at [Childhood Lekaemia Investigation Prague (**CLIP**)](https://clip.lf2.cuni.cz/en), where I worked with flow & CyTOF data, helping to develop [***tviblindi***](https://github.com/stuchly/tviblindi): an interactive trajectory inference tool powered by **persistent homology**.
This allowed to build multi-organ models of human B-cell development ([here](https://elifesciences.org/reviewed-preprints/95861)) and T-cell development ([here](https://onlinelibrary.wiley.com/doi/full/10.1002/eji.202451004)).

I started a collaboration with UCLouvain to I develop [***ViVAE***](https://github.com/saeyslab/ViVAE) and [***ViScore***](https://github.com/saeyslab/ViScore): a novel VAE-based **dimension-reduction** model with QC measures grounded in **differential geometry**, and a framework for evaluating embeddings of single-cell datasets.
Our manuscript ([here](https://www.biorxiv.org/content/10.1101/2023.11.23.568428v3)) is under review now.

Working with immunologists from the NIH, I designed and validated *iidx*: an end-to-end pipeline for large-scale statistical analysis of complex age- and sex-associated immunophe- notype changes, and put it to use with a 2196-donor flow cytometry data cohort.
We're releasing this soon.

<hr>
</details>

### My projects

I list some of my projects, including collaborations, below, sorted by category.

<details>
<summary>**Dimension reduction and structure learning**</summary>
<br>

#### [**ViVAE**](https://github.com/saeyslab/ViVAE)

Lower-dimensional mbedding framework that demonstrably **improves structure preservation, interpretability and QC in scRNA-seq dimensionality reduction**.
Using VAEs, a novel stochastic-MDS loss (based on [SQuadMDS](https://github.com/PierreLambert3/SQuaD-MDS-and-FItSNE-hybrid)) and data de-noising, we achieve a better balance of local and global structure preservation with scRNA-seq data.
Additionally, the model is equipped with a novel and generalisable algorithm for detecting latent space distortions (encoder indicatrices) and integrates with [FlowSOM](https://github.com/saeyslab/FlowSOM_Python).
I am the first author the associated manuscript, penned with my co-authors from Ghent University and UCLouvain (read current [pre-print](https://www.biorxiv.org/content/10.1101/2023.11.23.568428v3) here).
The work was presented at CYTO 2024.

#### [**GroupEnc**](https://github.com/saeyslab/GroupEnc)

*GroupEnc* is a proof-of-concept project for parametric multi-dimensional scaling (MDS) on GPU, presented at BNAIC/BeNeLearn 2023.
Check out the conference paper [here](https://bnaic2023.tudelft.nl/static/media/BNAICBENELEARN_2023_paper_46.9317ce00beb72bf31803.pdf).


<hr>
</details>

<details>
<summary>**Topological trajectory inference**</summary>
<br>

#### [**tviblindi**](https://github.com/stuchly/tviblindi)

*tviblindi* is a **semi-supervised single-cell TI tool** that uses TDA and **persistent homology** to work with high-dimensional data.
For my master thesis, I implemented parts of the TDA pipeline in C++ and created a **method for clustering trajectories based on persistent homology**, as well a **GUI in Shiny**.
The tool has since been applied successfully to create multi-organ models of development that refine descriptions of human [B-cell](https://onlinelibrary.wiley.com/doi/10.1002/eji.202451004) and [T-cell](https://elifesciences.org/reviewed-preprints/95861/figures) development.

<hr>
</details>

<details>
<summary>**Differential expression analysis**</summary>
<br>

#### **_iidx:_ Interpretable and interactive differential expression in cytometry**

*A public repository with a novel end-to-end pipeline for robust differential expression modelling in large flow cytometry data cohorts will soon be added.*
We're dealing with delays due to a publication freeze.

The work will be presented by me & Thomas Liechti at CYTO 2025.

#### [**tidycell**](https://github.com/davnovak/tidycell)

*tidycell* is a basic differential expression analysis tool written in R for cytometry data.
I developed during my time at [CLIP](https://clip.lf2.cuni.cz/cs).
It has been applied on GvHD data and in a project on head & neck cancers at [Biocev](https://www.biocev.eu/en).

<hr>
</details>

<details>
<summary>**Accelerating discovery in cytometry data**</summary>

### [**SingleBench**](https://github.com/saeyslab/SingleBench)

*SingleBench* will get you from data to discovery quicker.
It is an R framework for better interpretation of cytometry clustering, hyperparameter tuning & benchmarking.
I presented this work at CYTO 2021 and recently picked it up again and extended it.
Associated manuscript will be available soon.

<hr>
</details>

<details>
<summary>**Semi-automated single-cell data annotation**</summary>

#### [**hloss**](https://github.com/davnovak/hloss)

*hloss* is a work I presented at the ABLS 2022 bioinformatics conference.
It tackles the issue of evaluating cell type classification in single-cell data in a way that reflects known hierarchies and ontologies.
A novel scoring approach incorporates a biological prior to assess error based on degrees of relatedness.

#### [**SplitScore**](https://github.com/davnovak/SplitScore)

Work in progress on alternatives to hierarchical metaclustering done by [FlowSOM](https://github.com/saeyslab/FlowSOM).
Clusters are merged so as to preserve reasonable signal distributions per channel.
In practice, this can be done through preserving unimodality of marker expression (for cytometry data).
This is an ongoing effort, since the requirement of preserving some distribution modalities in metaclustering arises now and then in different projects.

<hr>
</details>

<details>
<summary><b>Evaluation & benchmarking of dimension reduction</b></summary>
<br>

#### [**ViScore**](https://github.com/saeyslab/ViScore)

*ViScore* is a collection of **evaluation metrics for dimensionality reduction** that address past problems with **fairness and scalability**.
Together with collaborators from UCLouvain, we have released a battery of both unsupervised and supervised evaluation algorithms and an **extensible HPC benchmarking framework**.
We build on **RNX curves** and the [**Neighbouhood Proportion Error**](https://github.com/akonstodata/NPE) to provide novel embedding-level and population-level scores.
This is described in our *ViVAE* [pre-print](https://www.biorxiv.org/content/10.1101/2023.11.23.568428v3).

We're incorporating some of the evaluation metrics from *ViScore* into [**TRACE**](https://github.com/aida-ugent/TRACE), which will be presented at CYTO 2025 by [Laura Hajzoková](https://github.com/laura-hajzokova).

<hr>
</details>

<details>
<summary><b>Utilities for computational cytometry</b></summary>
<br>

#### [**qctoy**](https://github.com/davnovak/qctoy)

*qctoy* is an R package for **simulating aberrances in flow cytometry measurements** that are relevant in designing QC tools and pipelines.
I developed this small tool during a summer internship at Saeys Lab to help with designing the QC algorithm what eventually became [**PeacoQC**](https://bioconductor.org/packages/release/bioc/html/PeacoQC.html).

#### [**auto_compensate**](https://github.com/davnovak/auto_compensate)

*auto_compensate* is an automated pipeline for large-scale **cytometry data compensation** I designed for [CLIP](https://clip.lf2.cuni.cz/cs).

</details>

<details>
<summary><b>Miscellaneous</b></summary>

#### [**hidden**](https://github.com/davnovak/hidden)

*hidden* is a hidden Markov model simulator in R.
I wrote it to understand HMMs better.

#### [**CommandLineParser**](https://github.com/katebrich/command_line_parser)

*CommandLineParser* is a C#/.NET API I co-wrote with [Kačka Břicháčková](https://github.com/katebrich).
This is a course project we teamed up for during our Master's in Bioinformatics at Charles University.

#### [**avl_tree**](https://github.com/davnovak/avl_tree)

*avl_tree* is an Adelson-Velsky and Landis tree implementation in Pascal.
It's some of my earliest code, written during my Bachelor's in Biology during which I took elective comp sci courses.

#### [**RCondaRun**](https://github.com/davnovak/RCondaRun)

*RCondaRun* is a tiny package for switching between Conda environments within a single R session when interfacing with Python.

<hr>
</details>
