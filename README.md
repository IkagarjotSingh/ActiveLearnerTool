Active Learning is a specialized version of semi supervised learning in which a learning algorithm is able to interactively query the user to obtain the desired labels at new data points. In this, we basically start with a small labelled training set and request labels for carefully selected instances. Newly labelled data points are added back to the training set and the process is repeated till the time we get all the data set labelled manually or intelligently. Manually labelled data points are the instances for which we request annotations from the manual annotator, while intelligently labelled data points are the ones for which prediction probability values are above a certain threshold value. 

In our approach, in order to sample the most uncertain data point or instance(s) for which we request the label information from manual annotator we used Pool-based sampling technique. In this approach, instances are queried in greedy fashion, according to informativeness measure used to evaluate all instances in the unlabeled data pool. We calculate the informativeness using Least Confidence Uncertainty Sampling method, which basically selects the instance with lowest confidence level to be labelled next.

This is a tool developed to process the requirements of a project. Input is the file with a pair of requirements and corresponding labels. The run-time parameters are provided in tool/ALParams.txt while all the descriptions related to the parameters are available in tool/ALParams-desc.txt

NLP pipeline -> Stop Words Removal, Count Vectorizer,Tfidf Transformation

Sample input files are available in static/data folder. While output files are available in static/data/logs folder for both binary and multiclass classification.
