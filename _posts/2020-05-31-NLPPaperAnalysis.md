---
layout: post
title: Quantitative Analysis and Trends of IWSSS Topics
subtitle: Using NLP to make the evolution of a research area and its topics visible 
share-img: "http://cdeck3r.github.io/img/blog/NLPPaperAnalysis_textanalysis.jpg"
bigimg:
  - "/img/blog/NLPPaperAnalysis_textanalysis.jpg" : "analytics information innovation communication (pixabay: xresch)"
---

As a scientist, I am constantly challenged by the fast progress of my research area. What are relevant papers I shall read? What are conference topics and how are papers distributed among them? In this blog, I demonstrate how to use NLP to automatically derive answers to such questions from publications.

Note, this is not an automated literature analysis. Nevertheless, some of the techiques may be utilized for it.

Directly go to the R notebook with the full analysis:  [IWSSSAnalysis.ipynb](https://github.com/cdeck3r/NLPPaperAnalysis/blob/master/notebooks/IWSSSAnalysis.ipynb)

## Motivational Example

Smart sensing system is an active research field involving expertise from many different areas ranging from sensor processing at one end to applications on the other end. In June 2019 I took part in the [International Workshop on Smart Sensing Systems (IWSSS)](https://iwsss19.github.io/). The workshop is a forum for exchange of experience among researchers from industry and academia actively involved in research, development and evaluation of smart sensing systems. IWSSS undergoes a permanent change of topics discussed throughout the last years. The group of authors changes as well as IWSSS may be the entry door for young researchers to enter the field and to get involved with the scientific community investigating smart sensing systems.

## Objectives and Research Questions

We believe, it is valueable to review the developments of the last years. The objectives are

* Make IWSSS content transparent across years
* Provide an repeatable approach to follow-up on future IWSSS occasions

Some typical research questions are:

* How to explore the papers' context to achieve a general understanding?
* What are strong relations connecting all documents with each other?
* What are relevant papers to read?
* What are topics and how do papers correspond to these topics?
* Topic evolution: How much are past topics still present in IWSSS?

## Approach

This analysis only utilizes titles and abstracts of paper publications. There are good reasons to focus on these both inputs. Firstly, titles and abstracts are available even when the paper is behind a paywall, secondly, they often come in formats easy to scrape and parse, e.g. from a website. PDF file content may get very hard to parse automatically, because of tables, formulas and images.

Using papers' titles and abstracts only, we are able to create a complete as possible data base for our analysis. We store the data in the MS Excel format to enable an easy way to manually edit this data base.

![analysis approach](https://github.com/cdeck3r/NLPPaperAnalysis/blob/master/approach.png)

We utilize qualitative and quantitative methods from NLP. A paper abstract or title refers to a document in NLP. The pile of papers form a document corpus, or simply corpus. The analysis uses the R language.

## Results

Let us start with some visualization. The following figure shows the word count network from stemmed abstracts. The stronger the line, the more often we find these (stemmed) words together.

![word count network](/img/blog/NLPPaperAnalysis_wordcountnetwork.png)

We can extend this approach and the plot the pairwise word correlation. This is basically the pearson correlation coefficient for words. When filterd for correlation coefficients above a threshold, the network reveals some interesting topic islands.

![word correlation network](/img/blog/NLPPaperAnalysis_wordcorrelationnetwork.png)

In the fowllowing we utilize tf-idf statistics to compile a paper reading list. The table dsiplays the Top-3 papers from this list. 

| title | important_words | median_tfidf |
|-------|--------|---------|
| Food Supply Chain Management System for Product History Using Blockchain | learn | 0.3915486 |
| System for motivating ethical consumption behavior using dongle interface application | ethic | 0.3433987 |
| Preference-Aware Video Summarization for Virtual Tour Experience | video | 0.3361408 |

We apply LDA topic modeling and show the distribution of per-document-per-topic probabilities $\gamma$ across the workshop years. The plot below shows boxplots for each topic and year. It marks the mean of $\gamma$ as blue point and the max of $\gamma$ as red triangle.

![topic modeling](/img/blog/NLPPaperAnalysis_topicmodelingyears.png)

Finally, let's list the papers from those topics which have dominated the workshops in 2016 and 2019.

| year | topic name | title |
|-------|--------|---------|
| 2016 | Smart Shop | Damage Detector: The Damage Automatic Detection of Compartment Lines Using A Public Vehicle and A Camera |
| 2016 | Smart Shop | Detecting Moving Objects Using Optical Flow with a Moving Stereo Camera |

It is imaginable from the titles that this classification is reasonable. However, this notebook just provides hints. 

## Take it with a Grain of Salt

Not all of them are correct. A user is still required to justify the recommendations. The table shows the papers from the topic "Recreation".

| year | topic name | title |
|-------|--------|---------|
| 2019 | Recreation | A Method for Generating Multiple Tour Routes Balancing User Satisfaction and Resource Consumption |
| 2019 | Recreation | An Approach for Measuring IoT Interoperability using Causal Modeling |

The paper "An Approach for Measuring IoT Interoperability using Causal Modeling" was co-authored by the notebook's author. It is unclear why this paper was classified into the Recreation topic. It definitely does not fit there.

So, always take an automatic analysis with a grain of salt.

## Resources

* [Repository](https://github.com/cdeck3r/NLPPaperAnalysis) on NLP Paper Analysis for reproducing this analysis 
* R notebook with the full analysis:  [IWSSSAnalysis.ipynb](https://github.com/cdeck3r/NLPPaperAnalysis/blob/master/notebooks/IWSSSAnalysis.ipynb)

