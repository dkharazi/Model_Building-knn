README

Note:
The code should take between 5-10 minutes to compile. Please be patient during code compilation. Thank you

Where to put input data (income dataset):
After opening the provided R code, the user should change the directory or the input data, which can be done by modifying the “read_csv” command on line 25. If the user changed the input data from a .csv format, he or she should change it back in order for the command to function properly. Additionally, the user should ensure the the “ggplot2,” “ROCR,” “pROC,” and “readr” packages are installed properly, in order to open/read the input data properly.

Where to find output data:
If each code block is run properly and orderly, four csv-formatted output files should be written to the user’s documents folder. The first file, named “JaccardSimilarityOutputTrain.csv,” is the output containing the top-k jaccard similarities for each entry of the training data. The second file, named “JaccardSimilarityOutputTest.csv,” is the output containing the top-k jaccard similarities for each entry of the testing data. The third file, named “OutputDataFrame.csv,” is the output containing the individual’s “ID,” the individual’s actual “class,” the individual’s predicted “class,” and the posterior probability regarding its predicted “class” of the testing data. The fourth file, named “OutputROCDataFrame.csv,” is the output containing the threshold, which is the accumulated posterior probability, True Positive value, False Positive value, True Negative value, False Negative value, True Positive Rate, and False Positive Rate given the threshold for each entry of the testing data. If these files aren’t found in the documents folder, the user’s options most likely follow a different routine. In this case, simply search for the file names in the search directory to locate each file.

How to interpret the output:
According to the general output data frame, each entry includes its “ID,” “Actual Class,” “Predicted Class,” and a posterior probability dependent on each observation’s proximity measure and value from the kNN algorithm. The first variable is labeled as “ID,” which is the given “ID” entries from the income training dataset. The “Actual Class” is each individuals actual “class” value from the training dataset. The “Posterior Probability” is based on each observation’s proximity measure from the kNN algorithm, which is based on the jaccard similarity values between each observation as a default. The “Predicted Class” is each individual’s predicted class given his or her posterior probability.

How to adjust the “k” variable:
An adjustable k is provided, but the user will need to adjust it by changing "k" on line 459. These lines are properly labeled, so the user shouldn't have an issue finding the adjustable "k" variable. The default for the "k" variable is 10.
