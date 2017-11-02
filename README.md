# Introduction
This repository contains code and documentation to study bias in data using some wikipedia articles on politicians from different countries. Supplemental data is used from Population Research Board's Country Population Data with population information as of mid-2015, as well as by getting an estimated quality score of articles using a publicly available Machine Learning Algorithm called ORES. The provenance information along with the Copyright and Licensing information is available in this README file. 

# Copyright and Licensing
NOTE: the code, text of this repository are governed by the MIT License included in the [LICENSE file](https://github.com/sumanbhagavathula/data-512-a2/blob/master/LICENSE)

The wikipedia articles data is available under the [Creative Commons BY](https://creativecommons.org/licenses/by/2.0/)
The ORES scores data is available under the [Creative Commons 0](https://creativecommons.org/publicdomain/zero/1.0/)
The PRB data is copyrighted and is not available and hence not included with this repo. You may choose to download this data directly from source that is mentioned in the Data Provenance section below.

# Overview
For this work, data on Wikipedia articles about policians from different countries is obtained from [figshare](https://figshare.com/articles/Untitled_Item/5513449) and scores for each of the article's referenced revision number is obtained by using the [ORES API](https://ores.wikimedia.org/v3/#!/scoring/get_v3_scores_context_revid_model)

In addition, Population information for various countries as of mid-2015 is obtained from the [Population Research Bureau (PRB) website](http://www.prb.org/DataFinder/Topic/Rankings.aspx?ind=14)

## Description of the process
The end to end process of this analysis work is broken down into three steps:

1. Data Acquisition
2. Data Processing
3. Analysis and Visualization

If any readers wants to reproduce the data acquisition step, they will need to download the wikipedia article data and the country population data and include them in the Raw Data Directory after cloning this repository.

## File structure
The source code, data (raw and processed) can be found in the following structure:

### Source
The source code is located in thie [github repo source code file](https://github.com/sumanbhagavathula/data-512-a2/blob/master/src/hcds-a2-bias.ipynb) and containing documentation and code for all the three steps mentioned above.

### Data
1. [Raw Data](https://github.com/sumanbhagavathula/data-512-a2/tree/master/src/data/raw) contains two CSV files, one with the wikipedia article data on politicians from different countries and the other is the article ORES score for the final revision of each of these articles. 

2. [Processed Data](https://github.com/sumanbhagavathula/data-512-a2/tree/master/src/data/processed) is a csv formatted processed data that has the combined article, population and ORES score data.


