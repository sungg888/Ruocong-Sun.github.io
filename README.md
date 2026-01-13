# Welcome to Ruocong Sun's Github Page!

<figure>
    <img src="https://github.com/sungg888/sungg888.github.io/blob/main/img/welcome.png?raw=true" width="220" height="220">
</figure>

# Technical Projects

## Automated Pricing Optimization System for Infinisia
**Due to confidentiality agreements, this project’s source code and proprietary data integrations cannot be made public.**

- **Project Overview:** This project focuses on building an automated, data-driven pricing optimization system for Infinisia’s Amazon US and Canada marketplaces. The system continuously evaluates SKU-level pricing performance using statistical experimentation and profit-based decision logic, enabling scalable, low-risk price optimization across hundreds of products.
- **Company Background:** Infinisia, headquartered in British Columbia, Canada, and established in 1997, operates with approximately 40 employees and primarily serves the US and Canadian markets, fulfilling 95% of orders. With recent expansion into Erlanger, Kentucky, Infinisia processes 2000 orders daily across platforms like Amazon, Walmart, and eBay. The company’s increased warehousing capacity supports its rapid growth.
- **Technical Implementation:**
    - The system integrates multiple production data sources, including Amazon daily sales data from BigQuery and live SKU metadata from internal OMS APIs. For each SKU, the tool establishes baseline performance windows and test windows, then applies statistical hypothesis testing (z-tests) to evaluate the impact of price changes on profit, units sold, sessions, and sales rank.  
    - A custom risk-scoring model combines profit uplift, profit-per-session, traffic changes, and rank movement to determine whether a price should be raised, reverted, or held. The system supports both FBA and FBM cost structures, incorporates Buy Box and inventory availability checks, and includes safeguards for zero-sales scenarios, stock-outs, and prolonged inconclusive tests.
    - All decisions, metrics, and state transitions are persisted via CSV and JSON state tracking, enabling reproducibility and historical analysis. A Flask-based dashboard consumes these outputs to provide executives with real-time visibility into price changes, profit impact, success rates, alerts, and year-over-year performance comparisons.
- **Results:** This pricing system enabled Infinisia to systematically test and deploy price increases while controlling downside risk, replacing ad-hoc manual pricing decisions with a statistically grounded experimentation framework. The solution improved pricing discipline, surfaced actionable insights at scale, and delivered measurable incremental profit gains, all while remaining interpretable to non-technical stakeholders through automated reports and dashboards.

---

## Forecasting model and logistic optimization model for Infinisia
**Due to the confidentiality agreement, this part of the GitHub repository cannot be made public.**

- **Project Overview:** This project focuses on optimizing inventory forecasting and replenishment for Infinisia by integrating data-driven forecasting models to enhance operational efficiency and stock management.
- **Company Background:** Infinisia, headquartered in British Columbia, Canada, and established in 1997, operates with approximately 40 employees and primarily serves the US and Canadian markets, fulfilling 95% of orders. With recent expansion into Erlanger, Kentucky, Infinisia processes 2000 orders daily across platforms like Amazon, Walmart, and eBay. The company’s increased warehousing capacity supports its rapid growth.
- **Technical Implementation:** This solution uses a deep learning approach built around a Long Short-Term Memory (LSTM) architecture to forecast sales for thousands of products across both Canadian and U.S. markets. The predictive framework is further augmented by an optimization model that integrates forecasted sales data with key variables such as current stock levels, lead times, and historical sales trends. By automating the decision of how much to order and when to order, the system ensures prompt replenishment while minimizing excess inventory. All calculations and processes connect seamlessly to a SQL database for real-time data management and streamlined decision-making.
- **Results:** Key outcomes of this initiative include improved forecast accuracy, reduced stockouts, optimized order placement, and enhanced operational efficiency. This robust, data-driven approach positions Infinisia to meet increasing customer demand while effectively managing inventory costs. And the forecasting model/tool was deployeed on server so users can use it with a user-friendly interface. 

---

## Evaluation model and AI agent for Autozen
**Due to the confidentiality agreement, this part of the GitHub repository cannot be made public.**

- **Project Overview:** The capstone project aims to enhance the used car market by refining vehicle price predictions and streamlining the sales process through proprietary predictive modeling and an AI negotiation agent, focusing on improving user satisfaction and operational efficiency.
- **Company Background:** Autozen, a digital startup, seeks to revolutionize the used car market by optimizing car valuations and the negotiation process, addressing information asymmetry with a data-driven solution to predict car prices accurately and improve transparency.
- **Technical Implementation:** The project employs data engineering and a log-normal regression model to predict car values, creating a pickle file and building an endpoint for Autozen to deploy the model. It also integrates LLM for explaining price predictions with coefficient explanations, alongside test files to ensure model functionality and a Flask dashboard for demonstrating the final product.
- **Results:** The main results are increased price prediction accuracy, streamlined auction and explanation processes, enhanced user experience, and reduced operational costs for Autozen.

---

## Red Wine Quality Prediction
[GitHub Repository](https://github.com/UBC-MDS/Red-Wine-Quality-Prediction)  
[Report](https://ubc-mds.github.io/Red-Wine-Quality-Prediction/red_wine_quality_prediction.html)

- This project involves using machine learning to predict wine quality on a scale from 0 to 10, based on its physiochemical properties. The best model (SVM RBF) achieved a final test set accuracy of approximately 62.3%.
- By employing a train-test split and cross-validation to ensure the model can handle unseen data. Various classification models were tested, including logistic regression, decision tree, kNN, and SVM RBF, to determine which offers the highest accuracy. This performance could be considered either modest or suboptimal depending on the expectations. A key observation is the model's difficulty in accurately predicting wines of extreme quality (either below 5 or above 6), indicating a lack of robustness to outliers.
- This project is reproducible by using a virtual environment or Docker container (provided in the GitHub repository).
- Optimized hyperparameters for algorithm models.

---

## Dream House Dashboard
[GitHub Repository](https://github.com/UBC-MDS/DSCI-532_2024_15_dreamhouse)  
[Dashboard](https://dsci-532-2024-15-dreamhouse.onrender.com/)

- This dashboard presents an interactive visualization of housing prices across the top 50 most populous cities in the United States of America. Our dashboard is built using the Dash package, enabling users to filter and explore the housing market data across various dimensions, such as state, city, house type, square footage, number of bedrooms and bathrooms, and more.
- The dashboard is designed to help display the key statistics of the real-estate market as well as a map of the selected area and a bar graph outlining the average price of listings in the selected area. The dashboard makes it easy to filter the data by state, city, square footage, price range, price per square foot, median household income of the zip code, number of bedrooms, and number of bathrooms. Once you have selected the criteria of your dream home, the dashboard will update to display the price of corresponding homes, their locations, and the summary statistics of all those homes that fit your selection.
- **Features:**
  - Interactive map visualizing average housing prices by region.
  - Filterable options for state and city selection.
  - Detailed pricing across top cities and a comparative list by states.
  - Visual representation of median house price, median square footage, and common home types.
  - Dynamic charts and graphs updating with user input.

**Preview:**
![Dreamhouse Demonstration](https://github.com/sungg888/Ruocong_Sun.github.io/blob/main/img/Dreamhouse%20Demostration.gif)

---

## GIC Calculator Python Package
[GitHub Repository](https://github.com/UBC-MDS/gic_calculator)  
[Readthedocs Report](https://gic-calculator.readthedocs.io/en/latest/)

- This project involves developing a Python package designed to assist users in understanding and analyzing the financial returns from Guaranteed Investment Certificates (GICs).
- The package focuses on calculating the interest returns over different investment periods, comparing these returns, and providing a visual representation of the differences. This utility will be particularly useful for investors and financial advisors who need to make informed decisions regarding GIC investments.
- **There are three functions in the package:**
  - `interest_calc(principal, term_length, gic_rate=None)`: Calculates the interest earned on a GIC after a specified number of years.
  - `calculate_gic_difference(term_length_n1, term_length_n2, principal, interest_rate1=None, interest_rate2=None)`: Calculates the difference in total returns (interest + principal) of a GIC between two different investment periods.
  - `gic_plotting(principal, term_lengths, gic_rates=None)`: Generates a bar plot to visually represent the difference in returns as calculated by `interest_calc`.

---

Let me know if you’d like to add or modify anything further!

