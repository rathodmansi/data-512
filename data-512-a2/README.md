# data-512 A2 - Identifying Bias in Data
  
## Goal
The goal of this assignment is to identify what, if any, sources of bias may exist in these datasets, and to develop testable hypotheses about how these biases might impact the behavior of machine learning models trained on the data, when those models are used for research purposes or to power data-driven applications. 

## License & Source Data
- This repository is under the MIT License [https://github.com/rathodmansi/data-512/blob/main/data-512-a2/LICENSE]
- Link to Wikimedia Foundation REST API terms of use : https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions

## Data Source & Methodology

There is a lot of information available online about the Wikipedia Talk corpus, and about the Perspective API. It ranges from traditional data, software, and product documentation to media articles and research papers. 

In order to determine whether the Wikipedia Talk corpus contains bias, the characteristics of that bias, and its potential consequences we have performed background research from the following website:

1. Overview of the research project that : https://meta.wikimedia.org/wiki/Research:Detox (Links to an external site.) 
2. Dataset description and schemas: https://meta.wikimedia.org/wiki/Research:Detox/Data_Release (Links to an external site.) 
3. Overview of Google’s Conversation AI project: https://conversationai.github.io/ (Links to an external site.) 


  #### Research Question Explored:

    <b>Analysis 1</b>:
    Research Question:<br>
    Does the Crowdflower worker's populations a balanced representation of gender, age-groups and education.Since the above datasets is from English Wikipedia,    therefore it will be interesting to see what is the distribution of workers amongst their first language spoken

    We will be analyzing the above trend for both our attack dataset and toxicity dataset. My motivation to include both the dataset in analysis is to have a complete picture of bias occuring or not occuring in both of these datasets.

    <b>Analysis Questions</b>
    Workers distribution across the following demographics:
    - gender,
    - age-group,
    - education and
    - first language spoken

## Directory Layout

- Data: This folder contains all the data files (.tsv) used for our analysis. These files are sourced from Figshare website
- Analysis: This contains the python notebook containing our research questions and the following analysis for bias
- Results: All the output figures generated during the analysis have been stored here
  
## Important Notes

- Please note that pageview api excludes any views done by bots or crawlers
- We have not excluded any missing value but instead replaced it as 'Unknown' data value.
