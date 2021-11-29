# gene_expression_analysis
# Microarray analysis with R
# step 1: normalization 
--using  Robust Multiarray Averaging (RMA) algorithm from the affy package;
# step 2: dimensionality reduction 
--by selecting the genes expressed in at least 5% of the samples, with a significantly different variance from the median variance of all sets of samples, 
then selecting genes differentially expressed having p_val < 0.05;
# step 3: correlation network analysis 
--applying the WGCNA package from the R language;
--the code for the correlation network analysis comes from the sources below and has been adapted for our objectives:
#https://rpubs.com/Amayrani/WGCNAPart1
#http://pklab.med.harvard.edu/scw2014/WGCNA.html
#http://pages.stat.wisc.edu/~yandell/statgen/ucla/WGCNA/wgcna.html
#https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/Tutorials/FemaleLiver-02-networkConstr-man.pdf
--find the hub genes in each module with the highest intramodular connectivity;
# step 4: create gene networks 
--with the igraph package in the R programming language;
