---
layout: page
permalink: /research_projects/
title: Research Interests
tagline: 
tags: 
modified: 01-28-2015
comments: false
image:
  feature: texture-feature-06.jpg
  <!-- credit: Arabidopsis contrast -->
---
# Overview

Biology is undergoing a data generating revolution with new data being generated faster than can be analyzed and fully understood in biologically meaningful ways. This is partly due to the emphasis on novel data sets rather than novel analyses and partly due to biologists being under trained in analysis, math and programming. As a biology community we should be developing models to understand the data that we already have and use the models to help us decide what experiments to do next. This theme has directed my research since I was an undergraduate. My graduate work focused on open questions in the climate change literature that also had implications for how crop and ecosystem models were parameterized or validated. Building on this background of plant carbon and nitrogen metabolism the current biological question I am interested in is plant competition. Specifically I am interested in how plants make metabolic trade-offs to compete for light resources above ground while also competing for nutrient and water resources below ground. To answer this question I am taking a systems genetics approach that leverages my background in whole plant physiology, metabolism, genomics and modeling. This approach allows me to scale from DNA polymorphisms to whole plant growth models using Bayesian statistics as a probabilistic glue across these scales. I think of the following descriptions as one large post-doc project partitioned out into four publishable units.

# Postdoc Project: Physiological Systems Biology of Competition in *Brassica rapa*
<img style="float: right" src="/images/research_overview.jpg">

### 1) *B. rapa* trait database
Hard won biological data (especially from the field) should not just sit in a lab note book or on spread sheets scattered across various machines. Sharing phenotypic data after publication should be a priority for us as a community, just like putting sequencing data into NCBI databases ([see Zamir (2013)](http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001595)). This allows for the data to be used to ask multiple questions, for modeling, or to be analyzed using systems biology techniques. Towards all these goals I have designed a graph database to house all of published trait data, experimental meta-data, publications, gene expression data, from the *B. rapa* population that I am working with combined with all the genomic features of the reference genome. 

A partial realization of this work has come out of working with an undergraduate [Tiffany Ho]() to create an interactive data visualization tool to examine co-occurrence of eQTL with physiological QTL called [QTLVisR](http://symposium.plb.ucdavis.edu/apps/qtl-visualization). This is still a work in progress, but the example does a great job showing the concept.

### 2) Multi-trait mapping with a dense genetic map

In collaboration with [Mike Covington](http://mfcovington.github.io/) (who generated the SNPs), I created a saturated genetic map for this population that can be found [here](https://github.com/rjcmarkelz/brassica_genetic_map_paper). This new map, along with a Bayesian statistical approach, my graph database, and *Brassica rapa* genome evolution information blends together into a very fun data science project. I am remapping all the published traits in the database using a multi-trait approach. This data is used directly in the next two aspects of my project. <img src="/images/genetic_map.jpg">

### 3) Multi-trait integration

I have been working on this aspect of my project the longest. The central dogma of molecular biology says DNA → RNA → Protein. Scaling the actions and interactions of proteins spatially across tissue or cell types is physiology. Scaling the actions of physiology across space and time is development. Updating the simple model to include physiology and development would look something like this: DNA → RNA → Protein → Physiology → Development. Of course there are feedbacks every step of the way, and it is hard to disentangle each of these into separate processes, but this simple conceptual model goes a long way. If there is a genomic location for these interactions explaining some of the variance observed in the physiological or developmental phenotype, then there is a QTL in that genomic location. QTL studies are conducted using genetic mapping populations where the parents of these populations are differ significantly from one another in the trait of interest. Up until recently, a majority of QTL studies have focused on traits that are the result of many proteins interacting one level of biological organization below the physiological or developmental trait. It is a large jump in biological organization to work backwards from physiology and development to DNA sequence differences. Assaying messenger RNA (mRNA) across a genetic mapping population can act as a stepping stone between the physiology and the DNA. mRNA contains rich amounts of information about the collective outputs of the cells assayed. Or to put it another way, mRNA can provide clues as to what proteins cells are planning to make given the current information from internal developmental and external environmental cues. The collection of mRNA expression is generally referred to as the gene co-expression network. I am interested in understanding the gene co-expression network and how it relates to DNA polymorphisms in one direction and physiological and developmental phenotypes in the other direction. In order to be able to do this, we not only need a good understanding of the biology, but we also need a good understanding of the ways in which these pieces of biological information fit together. I am working on the statistical techniques to connect these pieces of information in a probabilistic framework. This work is in collaboration with Upendra Devissety who did the bench work using a high-throughput RNA-seq library preparation technique.

### 4) Genetically informed *B. rapa* physiological growth model
<img src="/images/physiology_simulations.jpg">

Of course I do not want to just take all this data and make a large correlation matrix and try to infer meaning from it. I am using this data to parameterize physiologically based models of plant growth. Coming full circle to my PhD work in metabolism and physiology. This is my favorite part of my project. It involves integrating environmental time course data, physiological QTLs, and programming mathematical models of plant growth. Based on my meta-analysis results, and preliminary physiological modeling results, I choose a subset of genotypes to grow in the field for 2014 to test model predictions. I and three awesome undergrads are now working through this data. 

The other part of this project that motivates me is that I have 3 great undergrads working with me on it. 



#PhD Project

My PhD work focused on three open questions in the plant climate change literature all involving the effects of elevated atmospheric CO<sub>2</sub> on plants. 

### CO<sub>2</sub> Development Respiration- Arabidopsis - [paper](/pdfs/Markelz_etal_2014b.pdf)

### CO<sub>2</sub> Nitrogen Respiration- Arabidopsis - [paper](/pdfs/Markelz_etal_2014a.pdf)

### CO<sub>2</sub> Nitrogen Drought- Maize - [paper](/pdfs/Markelz_etal_2011.pdf)

#Equipment Projects
It is really enjoyable to build equipment. It pulls together many ways of thinking about biological problems. It forces the biologist to really think about what process they are trying understand and how to quantify it using some sort of sensor. These projects help biologists build intuition about measurement error, instrument limitation, methods development, materials selection, and design. These are skills that are undervalued in biology. 

#### 3D plant digitizer. Many of these methods are coming out now! Exciting times. I am working on this with some awesome undergrads. We have a prototype robot to collect this data for us, but we are looking forward to the summer break to really focus on getting this working. [video](https://vimeo.com/108757972)

#### Single leaf Arabidopsis respiration chamber/pipeline - Publications (see Arabidopsis thesis work)

#### Custom LICOR 6400 chamber head for soybean leaf respiration - [paper](/pdfs/Gillespie_etal_2012.pdf)

#### Fruitfly Respiration
I modified the Arabidopsis leaf chamber to accommodate little mesh bags of flys[paper](/pdfs/Walters_etal_2012.pdf)

#Undergraduate Thesis Project
#### How will elevated [CO<sub>2</sub>] alter soil and plant water status of the C<sub>3</sub>-crop soybean and the C<sub>4</sub>-crop maize? -[paper](/pdfs/Hussain_etal_2013.pdf)

