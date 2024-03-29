---
layout: page
permalink: /research_projects/
title: Postdoc Projects
tagline:
tags:
modified: 11-07-2017
comments: false
image:
  feature: texture-feature-06.jpg
  <!-- credit: Arabidopsis contrast -->
---

## Physiological Systems Biology of Competition in *Brassica rapa*

<figure>
	<img style="float: right" src="/images/research_overview.jpg">
</figure>

Plants growing in dense stands compete with one another for light resources at the top of the canopy. When plants sense neighbors through the phytochrome photoreceptor system they become apical dominant and grow upwards to maximize light capture. This response is termed shade avoidance and has very important ecological and agronomic consequences if plant resources are used for competitive growth instead of reproductive output. For example, overseeding in an agricultural field is wasteful of seed resources if many individuals die after competing with neighbors for limited light and nutrient resources. In ecological settings, mixed plant communities are competing for resources in a similar way to agricultural settings, but without the direct human management of inputs. In order to study the agronomic and ecological consequences of competition I am working with the emerging model species *Brassica rapa*. *B. rapa* is an ideal model for plant competition research because it has a sequenced genome, is both a crop and a weed in agricultural settings, and is a highly morphologically and physiologically diverse species. I am approaching this from many different angles that rely on my diverse research background and interests.

### 1) *B. rapa* trait database

<figure>
	<img  src="/images/graph_db.jpg">
</figure>

Hard won biological data (especially from the field) should not just sit in a lab note book or on spread sheets scattered across various machines. Sharing phenotypic data after publication should be a priority for us as a community, just like putting sequencing data into NCBI databases ([see Zamir 2013](http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001595)). This allows for the data to be used to ask multiple questions, for modeling, or to be analyzed using systems biology techniques. Towards all these goals I have designed a graph database to house all of the published trait data, experimental meta-data, publications, gene expression data, from the *B. rapa* population that I am working with combined with all the genomic features of the reference genome.

A partial realization of this work has come out of working with an undergraduate [Tiffany Ho](https://github.com/tiaho) to create an interactive data visualization tool to examine co-occurrence of eQTL with physiological QTL called [QTLVisR](http://symposium.plb.ucdavis.edu/apps/qtl-visualization). This is still a work in progress, but the example does a great job showing the concept.

### 2) Multi-trait mapping with a dense genetic map

In collaboration with [Mike Covington](http://mfcovington.github.io/) (who generated the SNPs), I created a saturated genetic map for this population that can be found [here](https://github.com/rjcmarkelz/brassica_genetic_map_paper). This new map, along with a Bayesian statistical approach and my graph database all blends together into a fun data science project. I am remapping all the published traits in the database using a multi-trait approach. This data is used directly in the next two aspects of my project. <img src="/images/genetic_map.jpg">

### 3) Trait data integration

I have been working on this aspect of my project the longest. The central dogma of molecular biology says DNA → RNA → Protein. Scaling the actions and interactions of proteins spatially across tissue or cell types is physiology. Scaling the actions of physiology across space and time is development. Updating the simple model to include physiology and development would look something like this: DNA → RNA → Protein → Metabolites → Physiology → Development. Of course there are feedbacks every step of the way, and it is hard to disentangle each of these into separate processes, but this simple conceptual model goes a long way. If there is a genomic location for these interactions explaining some of the variance observed in the physiological or developmental phenotype, then there is a QTL in that genomic location. QTL studies are conducted using genetic mapping populations where the parents of these populations are differ significantly from one another in the trait of interest. Up until recently, a majority of QTL studies have focused on traits that are the result of many proteins interacting one level of biological organization below the physiological or developmental trait. It is a large jump in biological organization to work backwards from physiology and development to DNA sequence differences. Assaying messenger RNA (mRNA) across a genetic mapping population can act as a stepping stone between the physiology and the DNA. mRNA contains rich amounts of information about the collective outputs of the cells assayed. Or to put it another way, mRNA can provide clues as to what proteins cells are planning to make given the current information from internal developmental and external environmental cues. The collection of mRNA expression is generally referred to as the gene co-expression network. I am interested in understanding the gene co-expression network and how it relates to DNA polymorphisms in one direction and physiological and developmental phenotypes in the other direction. In order to be able to do this, we not only need a good understanding of the biology, but we also need a good understanding of the ways in which these pieces of biological information fit together. I am working on the statistical techniques to connect these pieces of information in a probabilistic framework. This work is in collaboration with Upendra Devisetty who did the bench work using a high-throughput RNA-seq library preparation technique developed in the [Sinha Lab](http://www-plb.ucdavis.edu/labs/sinha/).

### 4) Genetically informed *B. rapa* physiological growth models

I am using this data to parameterize physiologically based models of plant growth. Coming full circle to my PhD work in metabolism and physiology. This is my favorite part of my project. It involves integrating environmental time course data, physiological QTLs, and programming mathematical models of plant growth. Based on my meta-analysis results, and preliminary physiological modeling results, I choose a subset of genotypes to grow in the field for 2014 to test model predictions. The field site I work at is home to three close collaborators at University of Wyoming: [Dr. Rob Baker](http://www.robertlbaker.org/Evolution_and_Development.html), Dr. Marc Brock, and [Dr. Cynthia Weinig](http://www.uwyo.edu/molecbio/faculty-and-staff/cyntia-weinig.html)

Here is a preview of a canopy scale model output predicting peak canopy N content for four different treatments. Notice that there is a clear interaction between N availability and crowding as to when there is peak canopy N. I am currently working on the physiology, metabolomics and RNA-seq samples with four great undergrads: Christina Day, Amanjot Kaur, Lakshmi Pabbisetty, and Neije Mukherjee-Roy.

<img src="/images/physiology_simulations.jpg">

In addition, I am developing a high-throughput 3D imaging robot and analysis pipeline to take non-destructive plant growth data for model calibration/validation. It is really enjoyable to build equipment. It pulls together many ways of thinking about biological problems. It forces the biologist to really think about what process they are trying understand and how to quantify it using some sort of sensor. These projects help biologists build intuition about measurement error, instrument limitation, methods development, materials selection, and design. These are skills that are undervalued in biology.

<figure>
	<img  src="/images/3D_summary.jpg">
</figure>

{% include _vimeoPlayer.html id="108757972" %}
