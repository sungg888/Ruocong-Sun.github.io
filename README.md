#### welcome to Ruocong Sun's Github page!
# Technical Projects 
## Red Wine Quality Prediction
#### [Github Repository](https://github.com/UBC-MDS/Red-Wine-Quality-Prediction)
#### [Report](https://ubc-mds.github.io/Red-Wine-Quality-Prediction/red_wine_quality_prediction.html)
#### - This project involves using machine learning to predict wine quality on a scale from 0 to 10, based on its physiochemical properties. The best model(SVM RBF) achieved a final test set accuracy of approximately 62.3%. 
#### - By employing a train-test split and cross-validation to ensure the model can handle unseen data. Various classification models were tested, including logistic regression, decision tree, kNN, and SVM RBF, to determine which offers the highest accuracy. This performance could be considered either modest or suboptimal depending on the expectations. A key observation is the model's difficulty in accurately predicting wines of extreme quality (either below 5 or above 6), indicating a lack of robustness to outliers.
#### - This project is reproducible by using a virtual environment or docker container(provided in GitHub repository)  
#### - Optimized hyperparameters for algorithm models.
<br>

## GIC Calculator Python Package
#### [Github Repository](https://github.com/UBC-MDS/gic_calculator)
#### [Readthedocs Report](https://gic-calculator.readthedocs.io/en/latest/)
#### - This project involves developing a Python package designed to assist users in understanding and analyzing the financial returns from Guaranteed Investment Certificates (GICs). 
#### - The package focuses on calculating the interest returns over different investment periods, comparing these returns, and providing a visual representation of the differences. This utility will be particularly useful for investors and financial advisors who need to make informed decisions regarding GIC investments.
#### - There are three functions in the package:
##### - interest_calc(principal, term_length, gic_rate=None): Calculates the interest earned on a GIC after a specified number of years.
##### - calculate_gic_difference(term_length_n1, term_length_n2, principal, interest_rate1=None, interest_rate2=None): Calculates the difference in total returns (interest + principal) of a GIC between two different investment periods.
##### - gic_plotting(principal, term_lengths, gic_rates=None): Generates a bar plot to visually represent the difference in returns as calculated by interest_calc.
