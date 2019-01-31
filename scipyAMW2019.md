# SciPy 2019

## Tutorial
### Short Description

This tutorial will cover the basics of phylogenetic computing in Python and Jupyter. Using a single dataset throughout the workshop, we will demonstrate to learners how to use Python and the RevNotebook to perform and summarize phylogenetic analysis. We will begin by using the Dendropy phylogenetic computing library to assemble datasets for phylogenetic analysis. We will then move on to discuss how to run Bayesian phylogenetic analysis in RevBayes via the Rev Jupyter kernel. Finally, we will discuss how to usefully summarize a posterior sample of trees and parameters in Python.

This tutorial will incorporate hands-on exercises in the Jupyter Notebook and the RevNotebook. These exercises will be interleaved with lecture-style teaching. 

## Instructors
Jeet Sukumaran: I am an assistant professor at San Diego State University, in the Biology Department. My research focus is computational evolutionary biology. I develop computational approaches for the study of the historical evolutionary relationships of organisms, to understand the processes that generate and structure the past, present, and even future patterns of life on our planet. My approaches are informed by a particular class of models called "phylogenies", which represent the relationships of life in terms of ancestor-descendent associations. I am one of the authors
of DendroPy, a Python library for phylogenetic computation. You can find out more about me, including links to my social media, code repositories, etc. at https://sukumaranlab.org.

April Wright: I am an assistant professor in Biology at Southeastern Louisiana University. My research focuses on incorporating fossils with molecular data for the inference of deep-time evolutionary relationships. In particular, I work with methods to estimate phylogenetic trees. This research enables me to ask both empirical, systematic questions about how organisms are related to one another, but also conceptual questions, such as how data sampling and preservation affect the quality of inference we can draw from biological data. As primarily undergraduate institution faculty, I also spend a lot of time considering how to deliver computational and statistical education to undergrad audiences. My lab website is at http://paleantology.com/.


## Skill level of participants

Due to time constraints, this tutorial cannot cover the basics of Python. We recommend that learners have familiarity with concepts such as for loops, functions, Pandas dataframes, and the Jupyter Notebook. We will introduce necessary library-specific syntax. 


| Time | Activity |
|------|----------|
| 0:15 | Welcome, outline, code of conduct |
| 0:15 - 0: 60 | [Download](https://dendropy.org/primer/reading_and_writing.html) a dataset from Treebase, [Add a sequence from GenBank](https://dendropy.org/primer/genbank.html), manage [taxon namespace](https://dendropy.org/primer/taxa.html) in Dendropy | 
| 1:00 - 1:15 | Break | 
| 1:15 - 3:15 | [Generate](https://revbayes.github.io/tutorials/) a tree in [RevBayes](https://revbayes.github.io/) using the [RevNotebook](https://github.com/revbayes/RevNotebooks)| 
| 3:15 - 4:00 | Visualize posterior in Pandas, assess convergence in PyMc, summarize consensus tree in Dendropy | 

##Details 

### 0:15 - 0:60

The first segment will cover the basics of phylogenetic terminology to ensure that everyone is using the same language to communicate in the course. Instructor Wright has previously delivered a similar lecture in at the [Analytical Paleobiology Workshop](http://www.analytical.palaeobiology.de/); this [lecture](https://github.com/wrightaprilm/APB2018/blob/master/TreeThinking.Rmd.Rpres) will be translated into Python. The lecture is a living lecture, in which slides will be made in the Jupyter Notebook and executed during the talk. Learners will have the slides in advance and be able to execute them as well. 

The next segment will be lead by instructor Sukumaran, who is the lead developer of the Dendropy phylogenetic computing library. Using Dendropy, learners will query a published dataset from Treebase, a free and open-source database of published phylogenetic matrices. Then, using Dendropy, we will query GenBank for an additional DNA sequence, and add it to the taxonomic dataset. This segment will consist of a brief lecture discussion of the Dendropy library, and how it is organized, followed by mostly hands-on practice of querying and managing data.


### 1:15 - 3:15

In this segment, we will estimate a phylogeny from the data we have collected. This will take place predominantly in [RevBayes](https://revbayes.github.io/) via the [RevNotebook](https://github.com/revbayes/RevNotebooks), a JupyterNotebook created using the [Rev kernel](https://github.com/revbayes/revbayes_kernel). This segment will be predominantly lead by Wright, who has contributed to both the Rev Kernel and the RevNotebook.

In this segment, we will discuss the basics of the [graphical model framework](https://revbayes.github.io/tutorials/intro_graph_models/) that underlies RevBayes' design philosophy. This segment will involve active learning with [magnets](https://twitter.com/WrightingApril/status/1027946335876599808) to assemble graphical models on the whiteboard. 

Following an orientation to the software design philosophy, we will actually estimate the tree, using a modification of [this tutorial](https://revbayes.github.io/tutorials/morph/). Learners will estimate a tree under several models of evolution, and compare their likelihood scores.

### 3:15 - 4:00

RevBayes produces two main outputs, a log file showing parameters of teh analysis sampled during the estimation, and a trees file, showing trees esimtated in the analysis. During the last segment of the tutorial, Sukumaran will show learners how to generate summary trees using Dendropy's [sumtrees](https://dendropy.org/programs/sumtrees.html) functions. We will also discuss visualizing posterior samples using Pandas and generating summary statistics from PyMC.


## Talk Schedule

| Time | Activity |
|------|----------|
| 0 - 7 minutes | What is phylogenetics? What can we learn from a phylogeny? How do biologists estimate phylogenies? |
| 7 -12 min | What makes teaching phylogenetics at the undergraduate level hard? |
| 12 - 17 minutes | What is the RevNotebook? |
| 17 - 24 minutes | What makes computational education hard in my specific context, and how do Jupyter Notebooks, JupyterHubs, and RevNotebooks help me overcome these barriers?  | 
| 24 - 25 min | Highlight ongoing work with the RevNotebook |

## Talk Short Summary: Delivering undergraduate phylogenetics education with Jupyter

Python and Project Jupyter enable computation to be integrated into teaching without making computation the focus of that teaching. In this talk, I will discuss how I use the Jupyter Notebook to deliver Bayesian phylogenetics training to undergraduate and Master's learners. I predominantly use the Rev Jupyter kernel to create phylogenetic modeling notebooks using the software RevBayes. Lastly, I will discuss how I have used JupyterHubs to serve students in a low-income state and overcome technical challenges associated with non-traditional students.

## Talk Abstract: Extending Jupyter Notebooks to deliver evolutionary biology to undergraduate learners

Evolutionary biology has always been tightly coupled with statistical inference and computational advances. This is especially true in phylogenetics, the practice of inferring evolutionary history from genetic and phenotypic data. Many interesting advances in phylogenetics come from development and application of new Bayesian models to describe the historical processes that generate observed biological data. 

However, bridging the gap between cutting-edge research and teaching undergraduates can be quite challenging. Very few undergraduate biologists have extensive experience with either computing or statistics. In the first part of this talk, I will discuss the use of Python and Jupyter Notebooks to teach students about evolutionary biology. I use Pandas and the Dendropy phylogentic computing library to introduce the basics of biological data management to students. 

Once students have comfort with Python and data management, we move on to phylogenetics and Bayesian modeling in a code-to-learn framework. In particular, I conduct my research in the software RevBayes. Recently, the RevBayes Jupyter kernel has been made available, facilitating the development of Jupyter notebooks for the Rev computing language. Rev is a general purpose, R-like language written in C++. It implements a graphical modeling framework for the construction of computational models for analysis of biological data.

Using the RevNotebook, I teach a series of tutorials spanning a range of topics from domain-agnostic Bayesian modeling to specific, complex phylogenetic models. Using the RevNotebook, novice students learn to understand Bayesian analyses, and to execute useful and meaningful biological workflows in the familiar interface of the Jupyter notebook. Biological computation is a fairly fragmented landscape, with biologists split between the use of R and Python. In this segment, I will also discuss some outstanding challenges with respect to the interoperability of RevNotebooks between the two languages.

Clear content is nothing without effective delivery mechanisms. One additional challenge for working with undergraduates is meeting the needs of diverse populations of students. Particularly for instructors in primarily undergraduate colleges and regional universities, student access to reasonable personal computers on which to learn and do homework is an issue, and can limit undergraduate participation in biological computing. I am faculty at Southeastern Louisiana University, which is located in a historically low-income region in a low-income state. The majority of students at Southeastern work more than 20 hours a week outside school. Many students are armed service reservists, or work other jobs that inhibit the use of a personal computer in off-hours. In the last part of the talk, I will discuss ways in which JupyterHubs can be leveraged to increase participation of non-traditional students in biological computation. In this section, I will also discuss advances within the State of Louisiana to make JupyterHubs more available for undergraduate education.