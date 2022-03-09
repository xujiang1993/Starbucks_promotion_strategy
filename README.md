# Starbucks promotion strategy analysis and optimization
This project uses AB test to validate the effectiveness of the existed promotion strategy and proposed an optimized promotion strategy to improve the business. 

Starbucks tries to stimulate consumer purchases by giving out promotional vouchers. The price of a specific product is assumed as $10. Since it costs the company average $0.15 to send out each promotion, it would be best to limit that promotion only to those that are most receptive to the promotion. Each data point includes one column indicating whether or not an individual was sent a promotion for the product, and one column indicating whether or not that individual eventually purchased that product. Each individual also has seven additional features associated with them, which are provided abstractly as V1-V7.

The data provided include the old promotion strategy records. The ab test found that although the promotion increased customer purchase rates, the profit indicator （Net Increamental Revenue） was negative. Therefore, the strategy needs to be improved. The second part of this project provides a simple machine learning classifier to optimize the strategy. The result turns that the optimized strategy can increase the NIR to a positive level when the IRR keep unchanged.

Although this project ends up with Gradient Boosting classifier, more useful classifiers can be used to further improve this strategy.

Techniques involved: 
* AB test
* classification

KPIs used:
* Increamental Response Rate (IRR)
* Net Increamental Revenue (NIR)

More details can be found in the Jupyter Notebook.
## Data
the data used in this project is sponsored by Starbucks. The total 120,000 records are collected and the data are divided in a 2:1 ratio and saved as two files: training set (training.csv) and test set (Test.csv).  

The data generally include user id (int), promotion (yes/no), purchase (1/0) and seven unknown parameters. 
## Package Requirement
The code was developed on python 3. The following packages are required:
* numpy
* pandas
* scipy
* scikit-learn
* matplotlib
* seaborn
## Licensing, Authors, Acknowledgements
I would like to thank Udacity for this amazing project, and Starbucks for providing the data.
