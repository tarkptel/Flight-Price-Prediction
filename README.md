<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
</head>
<body>

<h1 style="text-align: center; color: #2E86C1;">Flight Price Prediction</h1>

<p style="font-size: 1.2em;">Discover the power of machine learning in predicting flight prices with precision. This project aims to provide insights into airfare trends based on a wide range of features like airline, cities, travel class, and time of travel.</p>

<h2 style="color: #117A65;">Overview</h2>
<p>Flight prices are influenced by numerous factors, making them challenging to predict. This project leverages advanced machine learning models to forecast prices effectively, helping users make informed travel decisions.</p>

<h2 style="color: #117A65;">Dataset</h2>
<p>The dataset used for this project comprises various attributes:</p>
<ul>
    <li><strong>Airline</strong>: Name of the airline</li>
    <li><strong>Source City</strong>: City of departure</li>
    <li><strong>Destination City</strong>: City of arrival</li>
    <li><strong>Departure Time</strong>: Categorized into Morning, Afternoon, Evening, etc.</li>
    <li><strong>Arrival Time</strong>: Categorized into Morning, Afternoon, Evening, etc.</li>
    <li><strong>Stops</strong>: Number of stops during the journey</li>
    <li><strong>Class</strong>: Travel class (Economy or Business)</li>
    <li><strong>Price</strong>: Ticket price (Target variable)</li>
</ul>

<h2 style="color: #117A65;">Process</h2>
<p>To ensure the best model performance, we followed these steps:</p>
<ul>
    <li><strong>Data Cleaning</strong>:
        <ul>
            <li>Merged <strong>Morning</strong> and <strong>Early Morning</strong> into a single category.</li>
            <li>Merged <strong>Night</strong> and <strong>Late Night</strong> into single category.</li>
        </ul>
    </li>
    <li><strong>Encoding</strong>: Applied one-hot encoding to categorical columns such as airline, source city, and destination city.</li>
    <li><strong>Scaling</strong>: Used MinMaxScaler for normalizing the target column <strong>Price</strong>.</li>
    <li><strong>Feature Selection</strong>: Retained important features like stops, class, and departure time.</li>
    <li><strong>Modeling</strong>: Trained multiple machine learning models and fine-tuned hyperparameters using RandomizedSearchCV.</li>
</ul>

<h2 style="color: #117A65;">Modeling</h2>
<p>We explored and evaluated several models, including:</p>
<ul>
    <li>Linear Regression</li>
    <li>Random Forest Regressor</li>
    <li>XGBoost Regressor</li>
</ul>
<p>RandomizedSearchCV was employed for hyperparameter optimization to enhance model performance.</p>

<h2 style="color: #117A65;">Results</h2>
<p>The best-performing model achieved the following metrics:</p>
<ul>
    <li><strong>Mean Squared Error (MSE)</strong>: 0.0464</li>
    <li><strong>Root Mean Squared Error (RMSE)</strong>: 0.2156</li>
    <li><strong>R<sup>2</sup> Score</strong>: 0.95</li>
</ul>
<p>Analysis of feature importance revealed that <strong>stops</strong>, <strong>class</strong>, and <strong>departure time</strong> significantly impact flight prices.</p>

<h2 style="color: #117A65;">Installation</h2>
<pre>
<code>git clone https://github.com/your-username/flight-price-prediction.git
cd flight-price-prediction
pip install -r requirements.txt
</code>
</pre>

<h2 style="color: #117A65;">Usage</h2>
<ol>
    <li>Open the Jupyter Notebook file <code>Flight Price Prediction.ipynb</code>.</li>
    <li>Execute the notebook cells sequentially to preprocess data, train models, and evaluate predictions.</li>
    <li>Use the trained model to predict flight prices for new inputs.</li>
</ol>

<h2 style="color: #117A65;">Contributing</h2>
<p>We welcome contributions! Feel free to fork the repository, raise issues, or submit pull requests to improve the project.</p>

<h2 style="color: #117A65;">License</h2>
<p>This project is licensed under the <a href="https://opensource.org/licenses/MIT">MIT License</a>.</p>

<h2 style="color: #117A65;">Author</h2>
<p>Created by <strong>Tark Patel</strong>. Connect with me on <a href="https://www.linkedin.com/in/tark-patel">LinkedIn</a>.</p>

</body>
</html>
