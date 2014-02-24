Each row is a query-document pair. The first column is relevance label of this pair, the second column is
query id and the following columns are features of documents. The larger the relevance label, the more 
relevant the query-document pair. A query-document pair is represented by a 46-dimensional feature vector.
However, in this subset, we have extracted 6 features 43, 7, 6, 9, 8, 10 which are all zeros. So there is
a total of 40 features.


Report results for all the three folders of data.
Run the file as 
python <learn.py> <dir1> <dir2> <dir3>

This code will train a linear kernel sklearn SVM classifier with the training data set in each of the provided directories 
and then evaluate on the test sets provided in each of the corresponding directories.

At the end, it prints out the most significant features in each of the directory being classified and reports the accuracy 
of the classfication as a percentage.

This is done under requirement of CSCE 670 Information retrieval course
