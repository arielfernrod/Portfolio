# Predicting Growing Technologies
This project was part of my DataWorX II course at University of Silicon Valley. The project was titled the Big-Data Tripartite Project, so called because our team (in San Jose) was tasked with working alongside clients from Israel and Nepal to predict growing technologies, using 2020 Crunchbase data acquired by the clients. Due to copyright, I can't share the Crunchbase data, but the data can be acquired via Crunchbase (earlier data may be obtained at no cost).

Our team set out to prove or disprove a list of claims given by the clients using the given dataset.

## Claim
The claim of this project (henceforth referred to as Primary Claim or Claim 1) is that there is a positive correlation between the number of new companies in a particular field and among the growth of the field. 

This claim was revisited and joined together with another claim about the correlation of between the number of seed/pre-seed rounds in a field and among the growth of the field. 

Throughout this project, we will be using the terms technologies, verticals, fields, and categories interchangeably.

# Project Overview
This project works on the data provided by Crunchbase. The data given are CSV files 'organizations.csv' and 'funding_rounds.csv'. 'organizations.csv' contains over a million entries listing information about companies such as name, status, list of applicable categories, number of funding rounds, etc... 'funding_rounds' contains funding round information for some of the entries found in 'organizations.csv'. We will be using a versions of 'organizations.csv' and 'funding_rounds.csv' which have been filtered by a member of the team using a third-party application.


## File Descriptions
### claim_1_v1.ipynb - Version 1 of Claim 1
Here I computed the number of new companies per selected vertical per year in the category_list column of the 'organizations.csv' file.

### claim_1_v2.ipynb – Version 2 of Claim 1
Here I computed the number of new companies per selected vertical per year in the category_groups_list column.

### Primary-Claim_demo.ipynb – Final Version of Claim 1
This is the final notebook with all of my findings. Here I computed the number of new companies per selected vertical per year in the category_list column, the number of seed/pre-seed funding rounds per vertical per year, and the ratio between number of seed/pre-seed rounds and number of new companies per year. 

## Notes
In the final notebook, you can also uncomment the lines of code I have commented out under some of the statements, and comment out the matching statements above to see the data for 20 verticals instead of just the 10 we showcased. If you would like to plug in different verticals, matching filtered and merged funding rounds CSV files will need to be generated that contain the verticals you want to test out.