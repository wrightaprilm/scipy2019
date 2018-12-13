# SciPy 2019

## Tutorial

| Time | Activity |
|------|----------|
| 0:15 | Welcome, outline, code of conduct |
| 0:15 - 0:30 | Download a dataset from Treebase | 
| 0:30 - 1:00 | Add a sequence from GenBank, manage taxon namespace in dendropy | 
| 1:00 - 1:15 | Break | 
| 1:15 - 3:15 | Generate a tree in RevBayes | 
| 3:15 - 4:00 | Sumamrize tree in sumtrees, visualize posterior in Pandas, assess convergence in PyMc | 


## Talk Schedule

| Time | Activity |
|------|----------|
| 0 - 5 minutes | What is phylogenetics? How do we do it, usually? |
| 5 -10 min | What makes teaching phylogenetics at the undergraduate level hard? |
| 10 - 15 minutes | RevNotebook |
| 15 - 20 minutes | What makes use of RevNotebooks hard in my specific eduational context | 
| 20 - 25 min | JupyterHubs for us, sprint advert |

## Talk Short Summary: Delivering undergraduate phylogenetics education with Jupyter

Python and Project Jupyter enable computation to be integrated into teaching without making computation the focus of that teaching. In this talk, I will discuss how I use the Jupyter Notebook to deliver Bayesian phylogenetics training to undergraduate and Master's learners. I predominantly use the Rev Jupyter kernel to create phylogenetic modeling notebooks using the software RevBayes. Lastly, I will discuss how I have used JupyterHubs to serve students in a low-income state and overcome technical challenges associated with non-traditional students.

## Talk Abstract: Extending Jupyter Notebooks to deliver evolutionary biology to undergraduate learners

Evolutionary biology has always been tightly coupled with statistical inference and computational advances. This is especially true in phylogenetics, the practice of inferring evolutionary history from genetic and phenotypic data. Many interesting advances in phylogenetics come from development and application of new Bayesian models to describe the historical processes that generate biological data. 

However, bridging the gap between cutting-edge research and teaching undergraduates can be quite challenging. Very few undergraduate biologists have extensive experience with either computing or statistics. In the first part of this talk, I will discuss the use of Python and Jupyter Notebooks to teach students about evolutionary biology. I use Pandas and the Dendropy phylogentic computing library to introduce the basics of biological data management to students. 

Once students have comfort with Python and data management, we move on to phylogenetics and Bayesian modeling in a code-to-learn framework. In particular, I conduct my research in the software RevBayes. Recently, the RevBayes Jupyter kernel has been made available, facilitating the development of Jupyter notebooks for the Rev computing language. Rev is a general purpose, R-like language written in C++. It implements a graphical modeling framework for the construction of computational models for analysis of biological data.

Using the RevNotebook, I teach a series of tutorials spanning a range of topics from domain-agnostic Bayesian modeling to specific, complex phylogenetic models. Using the RevNotebook, novice students learn to understand Bayesian analyses, and to execute useful and meaningful biological workflows in the familiar interface of the Jupyter notebook. Biological computation is a fairly fragmented landscape, with biologists split between the use of R and Python. In this segment, I will also discuss some outstanding challenges with respect to the interoperability of RevNotebooks between the two languages.

Clear content is nothing without effective delivery mechanisms. One additional challenge for working with undergraduates is meeting the needs of diverse populations of students. Particularly for instructors in primarily undergraduate colleges and universities, student access to reasonable personal computers on which to learn and do homework is an issue, and can limit undergraduate participation in biological computing. I am faculty at Southeastern Louisiana University, which is located in a historically low-income region in a low-income state. The majority of students at Southeastern work more than 20 hours a week outside school. Many students are armed service reservists, or work other jobs that inhibit the use of a personal computer in off-hours. In the last part of the talk, I will discuss ways in which JupyterHubs can be leveraged to increase participation of non-traditional students in biological computation. In this section, I will also discuss advances within the State of Louisiana to make JupyterHubs more available for undergraduate education.