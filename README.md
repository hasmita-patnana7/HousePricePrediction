# HousePricePrediction
# Real Estate Price Prediction Website

## Project Overview

This project demonstrates the end-to-end process of building a real estate price prediction website. It involves creating a machine learning model using the Bangalore home prices dataset, deploying a Flask-based server to handle HTTP requests, and building a user interface with HTML, CSS, and JavaScript. The project covers key data science concepts such as data cleaning, outlier detection, feature engineering, dimensionality reduction, hyperparameter tuning with GridSearchCV, and cross-validation.

I completed this project as part of learning machine learning from the YouTube channel [Codebasics](https://www.youtube.com/channel/UCh9nVJoWXmFb7sLApWGcLPQ).

## Technology Stack

- **Python**: Primary programming language
- **Numpy & Pandas**: Data cleaning and manipulation
- **Matplotlib**: Data visualization
- **Sklearn**: Model building
- **Jupyter Notebook, Visual Studio Code, PyCharm**: Development environments
- **Flask**: Web server for handling HTTP requests
- **HTML/CSS/JavaScript**: Front-end development
- **AWS EC2**: Cloud deployment
- **Nginx**: Web server for serving the website


## Steps to Run the Project

### 1. Model Building

1. **Data Load and Cleaning**: Load the dataset and perform cleaning operations like handling missing values and removing outliers.
2. **Feature Engineering**: Create new features from existing ones to improve model performance.
3. **Dimensionality Reduction**: Apply techniques like PCA to reduce feature dimensions.
4. **Model Training**: Train the model using linear regression.
5. **Hyperparameter Tuning**: Use GridSearchCV for tuning model hyperparameters.
6. **Cross-Validation**: Validate the model using K-fold cross-validation.
7. **Model Saving**: Save the trained model to a file (`bangalore_home_prices_model.pkl`).

### 2. Flask Server

1. **Setup Flask**: Install Flask and required libraries.
2. **Create Server**: Develop a Flask server that loads the saved model and handles prediction requests.
3. **Endpoints**: Implement endpoints to serve the model predictions.

### 3. Front-End Development

1. **HTML**: Create the structure of the web page.
2. **CSS**: Style the web page.
3. **JavaScript**: Implement client-side logic to handle user input and communicate with the Flask server.

### 4. Deployment on AWS EC2

1. **Create EC2 Instance**: Set up an EC2 instance on AWS.
2. **Nginx Setup**: Install and configure Nginx to serve the web application.
3. **Deploy Code**: Copy the project files to the EC2 instance.
4. **Configure Nginx**: Point Nginx to the Flask server and set up routing.
5. **Install Python Packages**: Install required Python packages on the EC2 instance.
6. **Run Flask Server**: Start the Flask server to handle requests.

## Detailed Deployment Steps

### EC2 Instance Setup

1. **Create EC2 Instance**:
   - Use Amazon console to create an EC2 instance.
   - In the security group, add a rule to allow HTTP incoming traffic.

2. **Connect to Instance**:
   ```bash
   ssh -i "path_to_key.pem" ubuntu@ec2-instance-public-dns
   
# Nginx Setup

## Install Nginx:
```bash
sudo apt-get update
sudo apt-get install nginx
