<style>
  html, body {
    overflow-y: scroll;
  }
</style>
<p><code>davidnovak9000 at gmail dot com</code></p>
<p><a href="cv.pdf">CV</a> • <a href="https://scholar.google.com/citations?user=FU7FJPcAAAAJ&amp;hl=en">Google Scholar</a> • <a href="https://github.com/davnovak">GitHub</a> • <a href="https://www.linkedin.com/in/david-novak-04b65989">LinkedIn</a></p>
<p>Hi there! I&#39;m a <strong>bioinformatics and machine learning consultant</strong> working with <a href="https://burnslsc.com">Burns LSC</a> and a recent PhD grad.
I focus mostly but not exclusively on flow cytometry, CyTOF, bulk and single-cell RNA-seq, and other NGS data.
I have a track record in algorithm development as well as more data-driven analytical workflows.</p>

<p>During my PhD at <a href="https://saeyslab.sites.vib.be/en">Saeys Lab</a>, Flemish Institute of Biotechnology, I've advanced <strong>exploratory data analysis and statistical modelling of high-dimensional biological datasets</strong>.
I always put an emphasis on creating <strong>interactive solutions to keep domain experts in the loop</strong>.
I collaborate with immunologists, bioinformaticians, and computer scientists alike.</p>

<h4>I'm open to work, looking for interesting positions primarily (but not exclusively) in Canada.</h4>

<p>I am excited about <strong>responsible and interpretable AI and machine learning in biology</strong>.
At Ghent University, I have designed and taught practical sessions for over 200 post-grad students over 4 years, as well as guiding individuals and groups with their ML projects.
I also co-organised the inaugural <a href="https://training.vib.be/all-trainings/computational-cytometry-summer-school">Computational Cytometry Summer School</a>, guiding participants on statistical analysis within computational cytometry.</p>

<details>
<summary><b>My background</b></summary>

<ul>
<li>
A biology undergrad, I shifted toward bioinformatics a year into my studies, and went on to complete a Master and PhD in it.
</li>
<li>
My research started out at <a href="https://clip.lf2.cuni.cz/en">Childhood Lekaemia Investigation Prague (<b>CLIP</b>)</a>, where I worked with flow &amp; CyTOF data, helping to develop <a href="https://github.com/stuchly/tviblindi"><strong><em>tviblindi</em></strong></a>: an interactive trajectory inference tool powered by <strong>persistent homology</strong>.
This allowed to build multi-organ models of human B-cell development (<a href="https://elifesciences.org/reviewed-preprints/95861">here</a>) and T-cell development (<a href="https://onlinelibrary.wiley.com/doi/full/10.1002/eji.202451004">here</a>).
</li>
<li>
Then I secured a personal <a href="https://www.fwo.be/en/support-programmes/all-calls/phd/phd-fellowship-strategic-basic-research/">FWO Strategic Basic Research grant</a> and accepted a PhD position at <a href="https://saeyslab.sites.vib.be/en">Saeys Lab</a>, Center for Inflammation Research, which falls under the Flemish Institute of Biotechnology and Ghent University.
</li>
<li>
There I initiated a collaboration with UCLouvain to develop <a href="https://github.com/saeyslab/ViVAE"><strong><em>ViVAE</em></strong></a> and <a href="https://github.com/saeyslab/ViScore"><strong><em>ViScore</em></strong></a>: a novel VAE-based <strong>dimension-reduction</strong> model with QC measures grounded in <strong>differential geometry</strong>, and a framework for evaluating embeddings of single-cell datasets.
</li>
<li>
I also led a project in collaboration with immunologists from <a href="https://irp.nih.gov/pi/mario-roederer">Mario Roederer's lab</a> at the Vaccine Research Center, NIH.
I designed and validated <a href="https://github.com/saeyslab/iidx"><em>iidx</em></a>: an end-to-end pipeline for large-scale statistical analysis of complex age- and sex-associated immunophenotype changes, and put it to use with a 2196-donor flow cytometry data cohort.
We managed to put together the largest high-dimensional cytometry map of immune system changes linked to age and sex to date.
</li>
</ul>

<hr>
</details>

<h3 id="my-blog">Blog posts</h3>

I have a number of side projects, and sometimes I write blog posts where I showcase the work and discuss related matters that are interesting to me:

<ul>
<li>
<a href="https://davnovak.github.io/docs/cytoSNOW/vignette.html"><strong>Fast cytometry analysis with <i>cytoSNOW</i></strong></a> (2025-07-23)
</li>
</ul>

<h3 id="my-projects">My projects</h3>
<p>Below, I list some of my projects, including collaborations.
For most, the associated code and documentation are up on GitHub.
In some cases, the release of all materials is pending journal publication.</p>
<details>
<summary><b>Dimensionality reduction and structure learning</b></summary>

<h4><a href="https://github.com/saeyslab/ViVAE"><strong>ViVAE</strong></a></h4>

Lower-dimensional embedding framework that demonstrably <strong>improves multi-sacle structure preservation, interpretability, and QC in scRNA-seq dimensionality reduction</strong>.
Using VAEs, a novel stochastic-MDS loss (based on <a href="https://github.com/PierreLambert3/SQuaD-MDS-and-FItSNE-hybrid">SQuadMDS</a>), and data denoising, we achieve a better balance of local and global structure preservation.
Additionally, the model is equipped with a novel and generalisable algorithm for detecting latent space distortions (<strong>encoder indicatrices</strong>) and integrates with <a href="https://github.com/saeyslab/FlowSOM_Python">FlowSOM</a>.
I am the first author of the associated manuscript, which I penned with my co-authors from Ghent University and UCLouvain (under review at Cell Systems; read current <a href="https://www.biorxiv.org/content/10.1101/2023.11.23.568428v3">pre-print</a> here).
The work was presented at CYTO 2024.

<h4><a href="https://github.com/saeyslab/GroupEnc"><strong>GroupEnc</strong></a></h4>

<em>GroupEnc</em> is a proof-of-concept project for parametric multi-dimensional scaling (MDS) on the GPU, which I presented at BNAIC/BeNeLearn 2023.
Check out the conference paper <a href="https://bnaic2023.tudelft.nl/static/media/BNAICBENELEARN_2023_paper_46.9317ce00beb72bf31803.pdf">here</a>.


<hr>
</details>

<details>
<summary><b>Topological trajectory inference</b></summary>

<h4><a href="https://github.com/stuchly/tviblindi"><strong>tviblindi</strong></a></h4>

<em>tviblindi</em> is a <strong>semi-supervised single-cell TI tool</strong> that uses TDA and <strong>persistent homology</strong> to work with high-dimensional data.
For my master thesis, I implemented parts of the TDA pipeline in C++ and created a <strong>method for clustering trajectories based on persistent homology</strong>, as well as a <strong>GUI implemented in R Shiny</strong>, which allows the domain expert interrogate their datasets independently and at multiple resolutions.
The tool has since been applied successfully to create multi-organ models of development that refine descriptions of human <a href="https://onlinelibrary.wiley.com/doi/10.1002/eji.202451004">B-cell</a> and <a href="https://elifesciences.org/reviewed-preprints/95861/figures">T-cell</a> development.

<hr>
</details>

<details>
<summary><b>Differential expression analysis</b></summary>

<h4><a href="https://github.com/saeyslab/iidx"><strong><em>iidx:</em> interpretable and interactive differential expression in cytometry</strong></a></h4>

<i>iidx</i> is the most comprehensive workflow for pre-processing and differential expression analysis in large cytometry cohorts to date.
Thomas Liechti and I presented this work at CYTO 2025.
The repository already contains the code for reproducing our analysis.
The data will be available once the manuscript (which is underway) is published.

<h4><a href="https://github.com/davnovak/tidycell"><strong>tidycell</strong></a></h4>

<em>tidycell</em> is a basic differential expression analysis tool written in R for cytometry data.
I developed this during my time at <a href="https://clip.lf2.cuni.cz/cs">CLIP</a>.
It has been applied on GvHD data and in a project on head &amp; neck cancers at <a href="https://www.biocev.eu/en">Biocev</a>.
It is less elaborate than <i>iidx</i>, but it integrates <i>CellCnn</i> as an interesting approach to <strong>supervised feature extraction and addressing the multiple testing correction problem in smaller datasets</strong>.
This is done in addition to Wilcoxon ranked-sum testing of differential abundance.

<hr>
</details>

<details>
<summary><b>Accelerating discovery in cytometry data</b></summary>

<h4><a href="https://github.com/saeyslab/SingleBench"><strong>SingleBench</strong></a></h4>

<em>SingleBench</em> will get you from data to discovery quicker.
It is an R framework for <strong>better interpretation of cytometry clustering, hyperparameter tuning &amp; benchmarking</strong>.
In particular, <strong>it makes exploratory cluster analysis fast and clear</strong>.
It also allows you to test the influence of iterative data denoising (smoothing), which is poised to become more relevant as the dimensionality of cytometry data increases (with spectral and, to some extent, CyTOF).

<hr>
</details>

<details>
<summary><b>Semi-automated single-cell data annotation</b></summary>

<h4><a href="https://github.com/davnovak/hloss"><strong>hloss</strong></a></h4>

<em>hloss</em> is work that I presented at the ABLS 2022 bioinformatics conference.
It tackles the issue of <strong>evaluating cell type classification in single-cell data in a way that reflects known hierarchies and ontologies</strong>.
A novel scoring approach incorporates a biological prior to assess error based on degrees of relatedness.

<h4><a href="https://github.com/davnovak/SplitScore"><strong>SplitScore</strong></a></h4>

Work in progress on alternatives to hierarchical metaclustering done by <a href="https://github.com/saeyslab/FlowSOM">FlowSOM</a>.
Clusters are merged so as to preserve reasonable signal distributions per channel.
In practice, this can be done through <strong>preserving unimodality of marker expression, especially for markers that denote cell types (for cytometry data)</strong>.
This is an ongoing effort, since the requirement of preserving some distribution modalities in metaclustering arises now and then in different projects.

<hr>
</details>

<details>
<summary><b>Evaluation &amp; benchmarking of dimension reduction</b></summary>

<h4><a href="https://github.com/saeyslab/ViScore"><strong>ViScore</strong></a></h4>

<em>ViScore</em> is a collection of <strong>evaluation metrics for dimensionality reduction</strong> that address past problems with <strong>fairness and scalability</strong>.
Together with collaborators from UCLouvain, we have released a battery of both unsupervised and supervised evaluation algorithms and an <strong>extensible HPC benchmarking framework</strong>.
We build on <strong>RNX curves</strong> and the <a href="https://github.com/akonstodata/NPE"><strong>Neighbouhood Proportion Error</strong></a> to provide novel embedding-level and population-level scores.
This is described in our <em>ViVAE</em> <a href="https://www.biorxiv.org/content/10.1101/2023.11.23.568428v3">pre-print</a>.

We&#39;re incorporating some of the evaluation metrics from <em>ViScore</em> into <a href="https://github.com/aida-ugent/TRACE"><strong>TRACE</strong></a>, as presented at CYTO 2025 by <a href="https://github.com/laura-hajzokova">Laura Hajzoková</a>.

<hr>
</details>

<details>
<summary><b>Utilities for computational cytometry</b></summary>

<h4><a href="https://github.com/davnovak/cytoSNOW"><strong>cytoSNOW</strong></a></h4>

<em>cytoSNOW</em> takes the standard <a href="https://www.nature.com/articles/s41596-021-00550-0">FlowSOM protocol</a> and speeds it up, to work fast with big data.
I'm interested in <strong>making computational cytometry accessible to anyone, even without fancy hardware</strong>&mdash;this is a step in that direction.

I wrote up a small <a href="https://davnovak.github.io/docs/cytoSNOW/vignette.html">blog post</a> on my <i>cytoSNOW</i> workflow, showing how it gave a 4.6-fold speed-up in a large computational cytometry workflow on my laptop.

<h4><a href="https://github.com/davnovak/qctoy"><strong>qctoy</strong></a></h4>

<em>qctoy</em> is an R package for <strong>simulating aberrances in flow cytometry measurements</strong> that are relevant in designing QC tools and pipelines.
I developed this small tool during a summer internship in 2019 at SaeysLab to help with designing the QC algorithm what eventually became <a href="https://bioconductor.org/packages/release/bioc/html/PeacoQC.html"><strong>PeacoQC</strong></a>.

<h4><a href="https://github.com/davnovak/auto_compensate"><strong>auto_compensate</strong></a></h4>

<em>auto_compensate</em> is an automated pipeline for large-scale <strong>cytometry data compensation</strong> which I designed for <a href="https://clip.lf2.cuni.cz/cs">CLIP</a>.

<hr>
</details>

<details>
<summary><b>Miscellaneous</b></summary>

<h4><a href="https://github.com/davnovak/RCondaRun"><strong>RCondaRun</strong></a></h4>

<em>RCondaRun</em> is a tiny package for <strong>switching between Conda environments within a single R session when interfacing with Python</strong>.

<h4><a href="https://github.com/davnovak/hidden"><strong>hidden</strong></a></h4>

<em>hidden</em> is a hidden Markov model simulator in R.
I wrote it because I find HMMs fun and wanted to understand them better.

<h4><a href="https://github.com/katebrich/command_line_parser"><strong>CommandLineParser</strong></a></h4>

<em>CommandLineParser</em> is a C#/.NET API I co-wrote with <a href="https://github.com/katebrich">Kačka Břicháčková</a>.
This is a course project we teamed up for during our Master&#39;s in Bioinformatics at Charles University.

<h4><a href="https://github.com/davnovak/avl_tree"><strong>avl_tree</strong></a></h4>

<em>avl_tree</em> is an Adelson-Velsky and Landis tree implementation in Pascal.
It&#39;s some of my earliest code, written during my Bachelor&#39;s in Biology during which I took elective computer science courses.


<hr>
</details>
