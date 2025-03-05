<p><code>davidnovak9000 at gmail dot com</code></p>
<p><a href="cv.pdf">CV</a> • <a href="https://scholar.google.com/citations?user=FU7FJPcAAAAJ&amp;hl=en">Google Scholar page</a> • <a href="https://github.com/davnovak">GitHub page</a></p>
<p>Hi there! I&#39;m a <em>bioinformatician/computational biologist</em> and PhD researcher at <a href="https://saeyslab.sites.vib.be/en">Saeys lab</a>, Flemish Institute of Biotechnology in Belgium.
The focus of my PhD has been exploratory and statistical modelling of <strong>high-dimensional cytometry</strong> and <strong>single-cell RNA-seq data</strong>.
I love collaborating with immunologists, bioinformaticians and computer scientists alike, and <strong>delivering interpretable and interactive solutions to all the problems involved with big and complex data</strong>.
That includes effective presentation of results, complex data visualisation and designing graphical user interfaces to empower domain experts.</p>
<p>I enjoy teaching and tutoring, having co-taught <strong>machine learning</strong> at Ghent University for 4 years, which involved <strong>guiding over 200 students</strong> through practicals and helping them design and carry out semestral projects.
I also co-organised the successful <a href="https://training.vib.be/all-trainings/computational-cytometry-summer-school">Computational Cytometry Summer School 2024</a> where I taught statistical analyses of cytometry data.</p>
<p>I&#39;m proficient in <strong>R &amp; Python</strong> for data analysis and deeply familiar with <strong>high-dimensional cytometry and scRNA-seq data</strong>, having built and maintained large analytical pipelines, and written new algorithms to advance the state-of-the-art in interpretable single-cell analysis.
Other IT-related skills are listed in my <a href="cv.pdf">CV</a>.</p>
<details>
<summary><b>My background</b></summary>
<br>

A biology undergrad, I shifted toward bioinformatics a year into my studies, and went on to do a Master&#39;s and PhD in it (which I&#39;m finishing up now).

My research started out at <a href="https://clip.lf2.cuni.cz/en">Childhood Lekaemia Investigation Prague (<b>CLIP</b>)</a>, where I worked with flow &amp; CyTOF data, helping to develop <a href="https://github.com/stuchly/tviblindi"><strong><em>tviblindi</em></strong></a>: an interactive trajectory inference tool powered by <strong>persistent homology</strong>.
This allowed to build multi-organ models of human B-cell development (<a href="https://elifesciences.org/reviewed-preprints/95861">here</a>) and T-cell development (<a href="https://onlinelibrary.wiley.com/doi/full/10.1002/eji.202451004">here</a>).

I started a collaboration with UCLouvain to I develop <a href="https://github.com/saeyslab/ViVAE"><strong><em>ViVAE</em></strong></a> and <a href="https://github.com/saeyslab/ViScore"><strong><em>ViScore</em></strong></a>: a novel VAE-based <strong>dimension-reduction</strong> model with QC measures grounded in <strong>differential geometry</strong>, and a framework for evaluating embeddings of single-cell datasets.
Our manuscript (<a href="https://www.biorxiv.org/content/10.1101/2023.11.23.568428v3">here</a>) is under review now.

Working with immunologists from the NIH, I designed and validated <em>iidx</em>: an end-to-end pipeline for large-scale statistical analysis of complex age- and sex-associated immunophe- notype changes, and put it to use with a 2196-donor flow cytometry data cohort.
We&#39;re releasing this soon.

<hr>
</details>

<h3 id="my-projects">My projects</h3>
<p>I list some of my projects, including collaborations, below, sorted by category.</p>
<details>
<summary><b>Dimension reduction and structure learning</b></summary>
<br>

<h4><a href="https://github.com/saeyslab/ViVAE"><strong>ViVAE</strong></a></h4>

Lower-dimensional mbedding framework that demonstrably <strong>improves structure preservation, interpretability and QC in scRNA-seq dimensionality reduction</strong>.
Using VAEs, a novel stochastic-MDS loss (based on <a href="https://github.com/PierreLambert3/SQuaD-MDS-and-FItSNE-hybrid">SQuadMDS</a>) and data de-noising, we achieve a better balance of local and global structure preservation with scRNA-seq data.
Additionally, the model is equipped with a novel and generalisable algorithm for detecting latent space distortions (encoder indicatrices) and integrates with <a href="https://github.com/saeyslab/FlowSOM_Python">FlowSOM</a>.
I am the first author the associated manuscript, penned with my co-authors from Ghent University and UCLouvain (read current <a href="https://www.biorxiv.org/content/10.1101/2023.11.23.568428v3">pre-print</a> here).
The work was presented at CYTO 2024.

<h4><a href="https://github.com/saeyslab/GroupEnc"><strong>GroupEnc</strong></a></h4>

<em>GroupEnc</em> is a proof-of-concept project for parametric multi-dimensional scaling (MDS) on GPU, presented at BNAIC/BeNeLearn 2023.
Check out the conference paper <a href="https://bnaic2023.tudelft.nl/static/media/BNAICBENELEARN_2023_paper_46.9317ce00beb72bf31803.pdf">here</a>.


<hr>
</details>

<details>
<summary><b>Topological trajectory inference</b></summary>
<br>

<h4><a href="https://github.com/stuchly/tviblindi"><strong>tviblindi</strong></a></h4>

<em>tviblindi</em> is a <strong>semi-supervised single-cell TI tool</strong> that uses TDA and <strong>persistent homology</strong> to work with high-dimensional data.
For my master thesis, I implemented parts of the TDA pipeline in C++ and created a <strong>method for clustering trajectories based on persistent homology</strong>, as well a <strong>GUI in Shiny</strong>.
The tool has since been applied successfully to create multi-organ models of development that refine descriptions of human <a href="https://onlinelibrary.wiley.com/doi/10.1002/eji.202451004">B-cell</a> and <a href="https://elifesciences.org/reviewed-preprints/95861/figures">T-cell</a> development.

<hr>
</details>

<details>
<summary><b>Differential expression analysis</b></summary>
<br>

<h4><strong><em>iidx:</em> Interpretable and interactive differential expression in cytometry</strong></h4>

<em>A public repository with a novel end-to-end pipeline for robust differential expression modelling in large flow cytometry data cohorts will soon be added.</em>
We&#39;re dealing with delays due to a publication freeze.

The work will be presented by me &amp; Thomas Liechti at CYTO 2025.

<h4><a href="https://github.com/davnovak/tidycell"><strong>tidycell</strong></a></h4>

<em>tidycell</em> is a basic differential expression analysis tool written in R for cytometry data.
I developed during my time at <a href="https://clip.lf2.cuni.cz/cs">CLIP</a>.
It has been applied on GvHD data and in a project on head &amp; neck cancers at <a href="https://www.biocev.eu/en">Biocev</a>.

<hr>
</details>

<details>
<summary><b>Accelerating discovery in cytometry data</b></summary>

<h4><a href="https://github.com/saeyslab/SingleBench"><strong>SingleBench</strong></a></h4>

<em>SingleBench</em> will get you from data to discovery quicker.
It is an R framework for better interpretation of cytometry clustering, hyperparameter tuning &amp; benchmarking.
I presented this work at CYTO 2021 and recently picked it up again and extended it.
Associated manuscript will be available soon.

<hr>
</details>

<details>
<summary><b>Semi-automated single-cell data annotation</b></summary>
<br>

#### <a href="https://github.com/davnovak/hloss"><strong>hloss</strong></a>

<em>hloss</em> is a work I presented at the ABLS 2022 bioinformatics conference.
It tackles the issue of evaluating cell type classification in single-cell data in a way that reflects known hierarchies and ontologies.
A novel scoring approach incorporates a biological prior to assess error based on degrees of relatedness.

<h4><a href="https://github.com/davnovak/SplitScore"><strong>SplitScore</strong></a></h4>

Work in progress on alternatives to hierarchical metaclustering done by <a href="https://github.com/saeyslab/FlowSOM">FlowSOM</a>.
Clusters are merged so as to preserve reasonable signal distributions per channel.
In practice, this can be done through preserving unimodality of marker expression (for cytometry data).
This is an ongoing effort, since the requirement of preserving some distribution modalities in metaclustering arises now and then in different projects.

<hr>
</details>

<details>
<summary><b>Evaluation &amp; benchmarking of dimension reduction</b></summary>
<br>

<h4><a href="https://github.com/saeyslab/ViScore"><strong>ViScore</strong></a></h4>

<em>ViScore</em> is a collection of <strong>evaluation metrics for dimensionality reduction</strong> that address past problems with <strong>fairness and scalability</strong>.
Together with collaborators from UCLouvain, we have released a battery of both unsupervised and supervised evaluation algorithms and an <strong>extensible HPC benchmarking framework</strong>.
We build on <strong>RNX curves</strong> and the <a href="https://github.com/akonstodata/NPE"><strong>Neighbouhood Proportion Error</strong></a> to provide novel embedding-level and population-level scores.
This is described in our <em>ViVAE</em> <a href="https://www.biorxiv.org/content/10.1101/2023.11.23.568428v3">pre-print</a>.

We&#39;re incorporating some of the evaluation metrics from <em>ViScore</em> into <a href="https://github.com/aida-ugent/TRACE"><strong>TRACE</strong></a>, which will be presented at CYTO 2025 by <a href="https://github.com/laura-hajzokova">Laura Hajzoková</a>.

<hr>
</details>

<details>
<summary><b>Utilities for computational cytometry</b></summary>
<br>

<h4><a href="https://github.com/davnovak/qctoy"><strong>qctoy</strong></a></h4>

<em>qctoy</em> is an R package for <strong>simulating aberrances in flow cytometry measurements</strong> that are relevant in designing QC tools and pipelines.
I developed this small tool during a summer internship at Saeys Lab to help with designing the QC algorithm what eventually became <a href="https://bioconductor.org/packages/release/bioc/html/PeacoQC.html"><strong>PeacoQC</strong></a>.

<h4><a href="https://github.com/davnovak/auto_compensate"><strong>auto_compensate</strong></a></h4>

<em>auto_compensate</em> is an automated pipeline for large-scale <strong>cytometry data compensation</strong> I designed for <a href="https://clip.lf2.cuni.cz/cs">CLIP</a>.

<hr>
</details>

<details>
<summary><b>Miscellaneous</b></summary>
<br>

<h4><a href="https://github.com/davnovak/hidden"><strong>hidden</strong></a></h4>

<em>hidden</em> is a hidden Markov model simulator in R.
I wrote it to understand HMMs better.

<h4><a href="https://github.com/katebrich/command_line_parser"><strong>CommandLineParser</strong></a></h4>

<em>CommandLineParser</em> is a C#/.NET API I co-wrote with <a href="https://github.com/katebrich">Kačka Břicháčková</a>.
This is a course project we teamed up for during our Master&#39;s in Bioinformatics at Charles University.

<h4><a href="https://github.com/davnovak/avl_tree"><strong>avl_tree</strong></a></h4>

<em>avl_tree</em> is an Adelson-Velsky and Landis tree implementation in Pascal.
It&#39;s some of my earliest code, written during my Bachelor&#39;s in Biology during which I took elective comp sci courses.

<h4><a href="https://github.com/davnovak/RCondaRun"><strong>RCondaRun</strong></a></h4>

<em>RCondaRun</em> is a tiny package for switching between Conda environments within a single R session when interfacing with Python.

<hr>
</details>
