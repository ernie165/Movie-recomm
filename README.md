# Movie-recomm
Project Description
This project involves developing a movie recommendation system using collaborative filtering and deep learning. The system utilizes user ratings of movies to predict which movies a user is likely to enjoy. The recommendation model is implemented using TensorFlow and Keras and is wrapped in a web application using streamlit for user interaction. The main components of the project include:

Data Preparation:

The dataset is loaded from a CSV file containing columns 'userId', 'movieId', and 'rating'.
Unique user and movie IDs are mapped to continuous indices for embedding purposes.

Model Construction:

An embedding model is defined with separate embeddings for users and movies.
The dot product of these embeddings is computed and passed through a dense layer to predict the rating.
Training and Evaluation:

The dataset is split into training and testing sets.
The model is trained on the training set and evaluated on the testing set to ensure its performance.
Recommendation Function:

A function is provided to recommend top-N movies for a given user based on the trained model.
Web Application:

A Flask web application is set up with routes for the homepage and for handling recommendations.
The homepage allows users to input their user ID and the number of recommendations they want.
The recommendations are then displayed to the user.
1. Set Up Your Environment
Install Python: Make sure you have Python installed on your machine. You can check this by running python --version in your terminal. If Python is not installed, download and install it from the official Python website.

Install Necessary Packages: You’ll need to install Streamlit and any other dependencies your application requires, such as TensorFlow (for Keras) and PyMongo. You can do this using pip:

bash
Copy code
pip install streamlit keras pymongo numpy
2. Prepare Your Application Code
Create a new Python file (e.g., app.py) and paste the converted Streamlit code into it.

Make sure the trained model file (movie_recommender_model.keras) is in the same directory as your Python script or adjust the path in the code accordingly.

3. Run the Streamlit Application Locally
Open your terminal or command prompt and navigate to the directory where your app.py file is located.

Run the Streamlit application with the following command:

bash
Copy code
streamlit run app.py
Streamlit will start a local server and open a new tab in your default web browser, displaying your application.

4. Interacting with the Application
User ID: Enter the user ID in the provided input box.

Movie Name: Enter the name of the movie you want to predict the rating for.

Predict: Click the "Predict Rating" button to see the predicted rating based on your model.

The predicted rating will be displayed on the page. If the movie name is not found in your MongoDB database, an error message will be shown.

5. Deploying the Application Online
If you want to acce Streamlit application  over the internet, you can do so by doing the following:

 Streamlit Community Cloud
Sign Up/Sign In: Go to Streamlit Community Cloud and sign in with your GitHub account.
Create a New App:
Create a new repository on GitHub for your Streamlit application, and push your code (app.py and model file) to this repository.
In Streamlit Cloud, link your GitHub repository, select the branch, and specify app.py as the entry point.
Deploy: Streamlit will automatically build and deploy your app. Once deployed, you’ll receive a URL that you can share with others.



Youtube link: https://www.youtube.com/watch?v=13nVsivwQ1Y
