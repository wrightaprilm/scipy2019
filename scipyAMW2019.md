# SciPy 2019

## Tutorial
### Description

This tutorial will cover the basics of phylogenetic computing in Python. 


| Time | Activity |
|------|----------|
| 0:15 | Welcome, outline, code of conduct |
| 0:15 - 0:30 | [Download](https://dendropy.org/primer/reading_and_writing.html) a dataset from Treebase  | 
| 0:30 - 1:00 | [Add a sequence from GenBank](https://dendropy.org/primer/genbank.html), manage [taxon namespace](https://dendropy.org/primer/taxa.html) in Dendropy | 
| 1:00 - 1:15 | Break | 
| 1:15 - 3:15 | [Generate](https://revbayes.github.io/tutorials/) a tree in [RevBayes](https://revbayes.github.io/) using the [RevNotebook](https://github.com/revbayes/RevNotebooks)| 
| 3:15 - 4:00 | Visualize posterior in Pandas, assess convergence in PyMc | 


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