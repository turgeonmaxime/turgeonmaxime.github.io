+++
title = "Projects"
+++

Here is a list of current and former projects I have worked on. Also, here is a [blog post](https://www.maxturgeon.ca/blog/2018-09-28-what-i-currently-do/) describing some of the projects I worked on as a senior biostatistician with the Saskatchewan Health Authority.

## Missing data and matrix completion

Missing data is a common challenge in data science. As the number of measurements increases, so does the likelihood that at least one of them is missing for a given observation, leading to inefficient complete-case analyses. Matrix completion algorithms have gained popularity recently for their simplicity and computational efficiency. In this ongoing project, I developed a matrix completion algorithm based on generalized Singular Value Decomposition (SVD), which unlike classical SVD imposes constraints on the rows and columns of the data matrix. This framework is particularly suitable for multivariate methods like Weighted Principal Component Analysis and Correspondence Analysis.

## Anomaly detection

An MSc student in my research group (Neloy) has been investigating deep unsupervised learning models to detect anomalous observations in complex data (e.g. image data). Specifically, he reviewed several auto-encoder architectures to determine what characteristics provide the best performance. Based on these observations, he has been working on a new architecture that combines idea from the disentanglement literature with conditional graphical models.

In an ongoing project, I am using spectral clustering methods to detect bots in crowdsourcing platforms (e.g. Amazon's Mechanical Turk). In typical anomaly detection tasks, the anomalies are relatively rare compared to the normal data. In contrast, bots can represent a majority of the data collected from crowdsourcing platforms, which means it is crucial to identify and remove them from a dataset before analysis.

## Case-base sampling

In collaboration with [Sahir Bhatnagar](https://sahirbhatnagar.com/), we developed the R package [casebase](https://sahirbhatnagar.com/casebase/) which provides a flexible alternative framework for survival analysis. 

Our research groups then developed extensions of this framework to variable selection, competing risk analysis, and deep survival models.

## Dimension reduction for genomics and neuroimaging data

Genomics and neuro-imaging data have many common characteristics: they are high-dimensional (i.e. more features than data points) and they are highly structured. Indeed, because of various biological processes, there is typically a fair amount of correlation between the different features. This structure can be leveraged to increase computational and statistical efficiency of analytical methods.

In my PhD thesis, I explored this idea in the context of dimension reduction. Specifically, I combined Principal Component of Explained Variance (PCEV) with a block estimator of the residual covariance matrix to increase statistical efficiency. I also developed an empirical estimator for a high-dimensional test statistic that can be used with the traditional PCEV to improve the computational efficiency of region-based association tests.

More recently, a student in my research group (Czubrytt) looked at different covariance and precision matrix estimators, and how combining them with PCEV can improve statistical power. 

## Machine Learning for Molecule Design

This project is funded by a New Frontiers in Research Fund---Exploration grant. The goal is to use machine learning to identify structural factors of DNA nanomolecules that increase the likelihood of cell binding and cell entry. Potential applications include drug delivery. This work is in collaboration with [Katherine Bujold](https://experts.mcmaster.ca/display/bujoldk) and [Anthony Rullo](https://experts.mcmaster.ca/display/rulloa) from McMaster University.

## Shiny apps

Here is a non-exhaustive list of Shiny applications I have developed.

### Canadian Researcher PPE & Chemical Inventory

In collaboration with [Aleeza Gerstein](https://www.microstatslab.ca/), we developed a form through which researchers throughout Canada could advertise what kind of Personal Protective Equipment (PPE) they could donate---this was at the beginning of the COVID-19 pandemic. I then developed a Shiny application that would list all of the inventory that was available. The app is still available here: https://cancovid19ppe.shinyapps.io/cancovid19ppe/.

### Emergency Department Hourly Utilization

When working for the Saskatchewan Health Authority, there was a request to try to better understand the patient population that would visit the emergency department. The idea was to have, for each day, an hourly census of patients at different stages of their ED journey (arrival, physician initial assessment, admission to an inpatient unit, and discharge from ED). I developed an interactive report summarising this information. A mock version (i.e. with fake data) is available online: https://turgeonmaxime.shinyapps.io/EDutilization/.

