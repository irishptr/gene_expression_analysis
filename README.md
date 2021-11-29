# gene_expression_analysis
Microarray analysis with R
step 1: normalization using  Robust Multiarray Averaging (RMA) algorithm from the affy package;
step 2: dimensionality reduction by selecting the genes expressed in at least 5% of the samples, with a significantly different (higher) 
variance from the median variance of all sets of samples, then selecting genes differentially expressed having p_val < 0.05;
step 3: correlation network analysis applying the WGCNA package from the R language;
step 4: find the hub genes in each module with the highest intramodular connectivity;
step 5: create gene networks with the igraph package in the R programming language;
