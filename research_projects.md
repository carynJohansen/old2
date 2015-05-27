---
layout: page
permalink: /research_projects/
title: Research Projects
tagline: 
tags: 
modified: 01-28-2015
comments: false
image:
  feature: texture-feature-06.jpg
  <!-- credit: Arabidopsis contrast -->
---

Biology is undergoing a data generating revolution with data being generated faster than can be analyzed and understood in biologically meaningful ways. This is partly due to the emphasis on novel data sets rather than novel analyses and partly due to biologists being under trained in analysis, math and programming. There should be more of an emphasis on developing models to understand the data that we already have. In turn, these models should be updated according to new evidence and will help to decide what experiments to do next. Of course these models can be conceptual, statistical, or empirical but having a common framework to work in is the most important part. This is especially true when dealing with interactions. Interactions is a theme that has directed my research since I was an undergraduate. My graduate work focused on basic questions in the climate change literature dealing with environmental and developmental interactions effecting plant carbon and nitrogen metabolism. 
<figure>
	<img style="float: right" src="/images/research_overview.jpg">
</figure>
Building on this background the current biological question I am interested in is plant competition. Specifically I am interested in how plants make metabolic trade-offs to compete for light resources above ground while also competing for nutrient and water resources below ground. To answer this question I am taking a systems genetics approach that leverages my background in whole plant physiology, metabolism, genomics and modeling. This approach allows me to scale from DNA polymorphisms to whole plant growth models using Bayesian statistics as the probabilistic glue across these scales. The following is a description of my current postdoc projects with some summaries of my graduate work and equipment projects for background. 

# Postdoc Project: Physiological Systems Biology of Competition in *Brassica rapa*
<figure>
	<img  src="/images/graph_db.jpg">
</figure>


### 1) *B. rapa* trait database
Hard won biological data (especially from the field) should not just sit in a lab note book or on spread sheets scattered across various machines. Sharing phenotypic data after publication should be a priority for us as a community, just like putting sequencing data into NCBI databases ([see Zamir (2013)](http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001595)). This allows for the data to be used to ask multiple questions, for modeling, or to be analyzed using systems biology techniques. Towards all these goals I have designed a graph database to house all of published trait data, experimental meta-data, publications, gene expression data, from the *B. rapa* population that I am working with combined with all the genomic features of the reference genome. 

A partial realization of this work has come out of working with an undergraduate [Tiffany Ho]() to create an interactive data visualization tool to examine co-occurrence of eQTL with physiological QTL called [QTLVisR](http://symposium.plb.ucdavis.edu/apps/qtl-visualization). This is still a work in progress, but the example does a great job showing the concept.

### 2) Multi-trait mapping with a dense genetic map

In collaboration with [Mike Covington](http://mfcovington.github.io/) (who generated the SNPs), I created a saturated genetic map for this population that can be found [here](https://github.com/rjcmarkelz/brassica_genetic_map_paper). This new map, along with a Bayesian statistical approach, my graph database, and recently published *Brassica rapa* genome evolution by other groups all blends together into a fun data science project. I am remapping all the published traits in the database using a multi-trait approach. This data is used directly in the next two aspects of my project. <img src="/images/genetic_map.jpg">

### 3) Trait data integration

I have been working on this aspect of my project the longest. The central dogma of molecular biology says DNA → RNA → Protein. Scaling the actions and interactions of proteins spatially across tissue or cell types is physiology. Scaling the actions of physiology across space and time is development. Updating the simple model to include physiology and development would look something like this: DNA → RNA → Protein → Physiology → Development. Of course there are feedbacks every step of the way, and it is hard to disentangle each of these into separate processes, but this simple conceptual model goes a long way. If there is a genomic location for these interactions explaining some of the variance observed in the physiological or developmental phenotype, then there is a QTL in that genomic location. QTL studies are conducted using genetic mapping populations where the parents of these populations are differ significantly from one another in the trait of interest. Up until recently, a majority of QTL studies have focused on traits that are the result of many proteins interacting one level of biological organization below the physiological or developmental trait. It is a large jump in biological organization to work backwards from physiology and development to DNA sequence differences. Assaying messenger RNA (mRNA) across a genetic mapping population can act as a stepping stone between the physiology and the DNA. mRNA contains rich amounts of information about the collective outputs of the cells assayed. Or to put it another way, mRNA can provide clues as to what proteins cells are planning to make given the current information from internal developmental and external environmental cues. The collection of mRNA expression is generally referred to as the gene co-expression network. I am interested in understanding the gene co-expression network and how it relates to DNA polymorphisms in one direction and physiological and developmental phenotypes in the other direction. In order to be able to do this, we not only need a good understanding of the biology, but we also need a good understanding of the ways in which these pieces of biological information fit together. I am working on the statistical techniques to connect these pieces of information in a probabilistic framework. This work is in collaboration with Upendra Devissety who did the bench work using a high-throughput RNA-seq library preparation technique.

### 4) Genetically informed *B. rapa* physiological growth models

Of course I do not want to just take all this data and make a large correlation matrix and try to infer meaning from it. I am using this data to parameterize physiologically based models of plant growth. Coming full circle to my PhD work in metabolism and physiology. This is my favorite part of my project. It involves integrating environmental time course data, physiological QTLs, and programming mathematical models of plant growth. Based on my meta-analysis results, and preliminary physiological modeling results, I choose a subset of genotypes to grow in the field for 2014 to test model predictions. Here is a preview of a model output predicting peak canopy N content for four different treatments. Notice that there is a clear interaction between N availability and crowding as to when there is peak canopy N. I am currently working on the physiology, metabolomics and RNA-seq samples with four great undergrads: Christina Day, Amanjot Kaur, Lakshmi Pabbisetty, and Neije Mukherjee-Roy.
<img src="/images/physiology_simulations.jpg">
In addition, we are working on developing a high-throughput [3D imaging](https://vimeo.com/108757972) robot and analysis pipeline to take non-destructive plant growth data for model calibration/validation. 
<figure>
	<img  src="/images/3D_summary.jpg">
</figure>






