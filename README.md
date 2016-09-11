# RTB contest data analysis
Exploratory analysis of iPinYou RTB contest dataset

Dataset
-------
This repository contains only small data sample. The entire dataset is available at:
http://contest.ipinyou.com/data-release.html

Simple exploratory data analysis http://arxiv.org/pdf/1407.7073v2.pdf

Data description
-------

| Advertiser ID | Contest Season | Industrial Category |
| --- | --- | --- |
| df6f61b2409f4e2f16b6873a7eb50444 | 1 | Consumer Packaged Goods (CPG) |
| 3a7eb50444df6f61b2409f4e2f16b687 | 1 | Chinese vertical e-commerce |
| 9f4e2f16b6873a7eb504df6f61b24044 | 1 | Vertical online media |
| 1458 | 2 | Chinese vertical e-commerce Software |
| 3358 | 2 | Software |
| 3386 | 2 | International e-commerce |
| 3427 | 2 | Oil |
| 3476 | 2 | Tire |
| 2259 | 3 | Milk powder  |
| 2261 | 3 | Telecom |
| 2821 | 3 | Footwear |
| 2997 | 3 | Mobile e-commerce app install |

Sample preparation scripts
-------

Extract only the lines regarding advertiser ID 2261 (23rd column)

    head -5 imp.20131027.txt | awk -F $'\t' '$23 == "2261"'
    
Analysis:
------
* [Impression cleaning and analysis](https://nemusa.github.io/rtb_data_mining/raw_data_cleaning)

