# Movie-recomm
Project Description
This project involves developing a movie recommendation system using collaborative filtering and deep learning. The system utilizes user ratings of movies to predict which movies a user is likely to enjoy. The recommendation model is implemented using TensorFlow and Keras and is wrapped in a web application using Flask for user interaction. The main components of the project include:

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

Hosting the Application
1.Install Required Libraries:
Ensure you have Python and pip installed. You will also need to install the required libraries.

bash
pip install pandas numpy tensorflow flask scikit-learn
2.Prepare Your Script:
Make sure your script is in the proper directory. The script should look like the one you've provided, with your dataset path correctly specified.

3.Set Up the Directory Structure:
Organize your project directory. It should include:

app.py: Your main Flask application script.
templates/: A folder containing your HTML templates (index.html and recommendations.html).
static/: A folder containing any static files like CSS or JavaScript files, if needed.
ratings.csv: Your dataset file.
4.Create HTML Templates:
Create the index.html and recommendations.html files inside the templates/ folder. 

5. Run the application

6.Open Browser:
After running python app.py, open your browser and go to http://127.0.0.1:5000/.

Use the Application:
Enter a user ID and the number of recommendations you want, then submit the form to see the recommendations.

Youtube link: 
