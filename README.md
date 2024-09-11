# car-price-predictor


Car Price Predictor
Overview
The Car Price Predictor is a web application that predicts the price of a car based on user inputs using a pre-trained linear regression model. The application is built using Flask and provides a simple web interface for users to enter car details and receive price predictions.

Project Structure
README.md: This file.
main.py: The main Python script that runs the Flask application.
LinearRegressionModel.pkl: Pre-trained linear regression model used for predictions.
Cleaned2_Car_data.csv: Dataset used to train the model, containing car features.
data.json: (Not used in the provided code but might be for future use or additional features.)
index.html: HTML template for the web interface.
static.css: CSS file for styling the web interface.
misc.xml, modules.xml, vcs.xml, workspace.xml: Project configuration files.
Installation
To set up the Car Price Predictor on your local machine, follow these steps:

Clone the Repository:

bash
Copy code
git clone <repository-url>
cd car-price-predictor
Set Up a Virtual Environment (optional but recommended):

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install Required Packages: Ensure you have Flask, Flask-CORS, and other dependencies installed. You can use the following command to install them:

bash
Copy code
pip install Flask Flask-Cors pandas numpy scikit-learn
Run the Application:

bash
Copy code
python main.py
This will start the Flask development server.

Usage
Access the Web Interface: Open your web browser and navigate to http://localhost:5000. You will see a form where you can input details about the car.

Enter Car Details:

Company: Select the car manufacturer from the dropdown.
Car Model: Choose the specific model of the car.
Year: Select the year of manufacture.
Fuel Type: Choose the type of fuel used by the car.
Kms Driven: Enter the number of kilometers driven.
Get Price Prediction: After submitting the form, the application will display the predicted price of the car based on the provided details.

How It Works
Model Loading: The pre-trained model is loaded from LinearRegressionModel.pkl using pickle.

Data Handling: The car features are read from Cleaned2_Car_data.csv, which includes information about car companies, models, years, and fuel types.

Prediction: When a user submits the form, the application creates a DataFrame with the input values and uses the loaded model to predict the car's price.

Results: The predicted price is displayed to the user in the web interface.

Contributing
If you would like to contribute to this project, please fork the repository and submit a pull request with your proposed changes. Ensure that your contributions include appropriate tests and documentation.

