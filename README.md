# Iris-Data-T-Stat-Mutual-Info-score
In the code above, we first load the Iris dataset using pandas. Then we create a matrix of scatter plots for each pair of the four features using the scatter_matrix() function from pandas' plotting module. We set the diagonal parameter to 'hist' to create histograms on the diagonal instead of scatter plots.

Next, we calculate the T-statistics for each pair of the four features using the ttest_ind() function from scipy.stats. We loop through each pair of features and calculate the T-statistic between the first 50 samples (Iris setosa) and the second 50 samples (Iris versicolor). We store the T-statistics in a matrix.

We also calculate the Mutual Information for each pair of the four features using the mutual_info_score() function from scikit-learn's metrics module. We loop through each pair of features and calculate the Mutual Information between the two features for all samples. We store the Mutual Information scores in a matrix.

Finally, we print the T-statistics and Mutual Information matrices. Note that we could also visualize these matrices using a heatmap, but I didn't include that in the code.
