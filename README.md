## welcome to Ruocong Sun's Github page!

<figure>
    <img src="https://github.com/sungg888/sungg888.github.io/blob/main/img/welcome.png?raw=true" width="220" height="220">
</figure>

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
<br>

## Dream House Dashboard
#### [Github Repository](https://github.com/UBC-MDS/DSCI-532_2024_15_dreamhouse)
#### [Dashboard](https://dsci-532-2024-15-dreamhouse.onrender.com/)
#### - This dashboard presents an interactive visualization of housing prices across the top 50 most populous cities in the United States of America. Our dashboard is built using the Dash package, enabling users to filter and explore the housing market data across various dimensions, such as state, city, house type, square footage, number of bedrooms and bathrooms, and more.
#### - The dashboard is designed to help display the key statistics of the real-estate market as well as a map of the selected area and a bar graph outlining the average price of listings in the selected area. The dashboard makes it easy to filter the data by state, city, square footage, price range, price per square foot, median household income of the zip code, number of bedrooms, and number of bathrooms. Once you have selected the criteria of your dream home, the dashboard will update to display the price of corresponding homes, their locations, and the summary statistics of all those homes that fit your selection.
#### - Features in dashboard
- Interactive map visualizing average housing prices by region.
- Filterable options for state and city selection.
- Detailed pricing across top cities and a comparative list by states.
- Visual representation of median house price, median square footage, and common home types.
- Dynamic charts and graphs updating with user input.
#### Preview
![](https://github.com/sungg888/Ruocong_Sun.github.io/blob/main/img/Dreamhouse%20Demostration.gif)
<br>

## Evaluation model and AI agent for Autozen
#### Due to the confidentiality agreement, this part of the GitHub repository cannot be made public.
#### - Project Overview: The capstone project aims to enhance the used car market by refining vehicle price predictions and streamlining the sales process through proprietary predictive modeling and an AI negotiation agent, focusing on improving user satisfaction and operational efficiency.
#### - Company Background: Autozen, a digital startup, seeks to revolutionize the used car market by optimizing car valuations and the negotiation process, addressing information asymmetry with a data-driven solution to predict car prices accurately and improve transparency.
#### - Technical Implementation: The project employs data engineering and a log-normal regression model to predict car values, creating a pickle file and building an endpoint for Autozen to deploy the model. It also integrates LLM for explaining price predictions with coefficient explanations, alongside test files to ensure model functionality and a Flask dashboard for demonstrating the final product.
#### - Results: The main results are increased price prediction accuracy, streamlined auction and explanation processes, enhanced user experience, and reduced operational costs for Autozen.
