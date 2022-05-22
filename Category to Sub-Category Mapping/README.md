# Category to Sub-Category Mapping
Creates sub-categories from categories assigned to entries in a Crunchbase dataset from 2013, which lists around 462k companies' information. Due to copyright, I can't include the dataset here.

## JUPYTER NOTEBOOK WORKFLOW
sub-category.ipynb => mnb-sc.ipynb => mnb.ipynb

## FILE DESCRIPTIONS
sub-category.ipynb : Main notebook. Reads in 'objects.csv', a Crunchbase dataset from 2013 listing 462k entries containing information about companies. This notebook produces a list of sub-categories for each entry, 'submapped.csv'.

submapped-cleaning.ipynb: Cleans 'submapped.csv'.

mnb-sc.ipynb : Reads in 'submapped.csv' and helps user manually create a training set to be used in Multinomial Naive Bayes model. This notebook produces 'test_set.csv'.

mnb.ipynb : Reads in 'test_set.csv' as the training set and tests it against 'submapped.csv' to train the MNB model.

submapped.csv : produced by sub-category.ipynb

test_set.csv : produced by mnb-sc.ipynb

submapped-MNB : final CSV produced by mnb.ipynb

cat_subcat.xlsx : category/sub-category pairs