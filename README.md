# GHZ_Quant_Paper_Research
A collection of Jupyter notebooks with a momentum focused analysis from a paper provided.

GHZ_RFS_Paper.pdf
This is the paper that the data used is based off. It contains explanation for the collection of 
the large number of independent factors.

Variable_Definitions.docx
Contains all long-form definitions of factors in analysis. Names are shortened in the actual data.

var_key.csv
This sheet contains a processed and dataframe friendly version of Variable_Definitions.docx. 
This is used in a function to get the longform definition easily within a notebook.

Returns_-_Value_weighted.csv
Returns_-_Equal_Weighted.csv
Provided sheets with factors provided from the paper. The equal weighted returns was used for the analysis. 

peqw.csv
Date processed version of Returns_-_Equal_Weighted.csv.

mom.csv
This sheet contains the nearly-fully processed factors for momentum analysis. The final processing 
for clustering is the standardization of each feature and is done in the jupyter notebooks provided.

Analysis_of_csvs.ipynb
pewq.ipynb
pewqknn.ipynb
These contain (in this order) subsequent analysis of the data given.
The first is initial data analysis, while the second is the first couple of models built to model momentum.
The third is a collection of classifiers to classify direction (positive/negative) of returns.

The models returned about the same fair perfomance, with a lack of an ability to predict negative return months. One
model returned higher success, but was ultimately found to be overfit and possibly inadequate.

Notes: The data split for cross validation was a simple random split and not a time-series split as is reccomended with
this type of data. This is due to a prior lack of experience at the time of analysis.
