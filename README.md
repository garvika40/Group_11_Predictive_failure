## Steps for Predictive Maintenance Project

#### Data Collection and Preprocessing
#### Data Visualization
#### Machine Learning Model Fitting and Evaluation
#### API Development with Flask
#### Containerization with Docker
#### Deployment

## Machine Learning Model Fitting
In predictive maintenance project, we trained various machine learning models to predict equipment failures based on historical data. The models used include Random Forest, Support Vector Machine (SVM), K-Nearest Neighbors (KNN), Logistic Regression, and XGBoost.


### Why XGBoost?

XGBoost was selected as the primary model for predictive maintenance project due to several compelling reasons:

- *Performance*: 

- *Robustness*: 

- *Flexibility*: 

- *Scalability*: 

- *Interpretability*: 

## Predictive Maintenance Web Application with Flask

*Model Placement*: Pre-trained machine learning model (xgb_model.pkl) is placed in the same directory as the Flask application script (app.py).

2. *Dependency Installation*: Flask and other required dependencies need to be installed.

3. *Running the Application*: Execute the Flask application script (app.py). This will start the Flask web server locally.

4. *Accessing the Web Interface*: Once the Flask application is running, can access the web interface by navigating to http://localhost:5000 in your web browser. 

## Containerization with Docker
Containerization with Docker allows us to package our predictive maintenance application along with its dependencies into a standardized unit called a container. This enables us to run the application seamlessly across different environments without worrying about compatibility issues.

#### Steps:
##### Docker Installation.
##### Dockerfile Creation.
##### Building the Docker Image.
##### Running the Docker Container.


## Deployment on Amazon EC2 Instance

### Steps:

1. *Amazon EC2 Setup*: 
   - Sign in to the AWS Management Console 
   - Launch a new EC2 instance with  Ubuntu Server 

2. *Connect to the EC2 Instance*: 
   - Use SSH to connect to your EC2 instance from local machine.
   - Can find the public IP address of instance in the EC2 dashboard.

3. *Transfer Files*: 
   - Transfer project files, including the Flask application script (app.py), the pre-trained model file (xgb_model.pkl),requirement file, frontend file (index.html), to the EC2 instance using SCP or SFTP.

4. *Install Docker*: 
   - Install Docker on your EC2 instance to containerize application and manage dependencies efficiently.

5. *Containerize with Docker*: 
   - Create a Dockerfile in the project directory to define application's environment and dependencies.
   - Build a Docker image and run a Docker container on EC2 instance using the same steps as described earlier.

6. *Access the Application*: 
   - Once the Docker container is running on your EC2 instance, access Flask application through the public IP address or domain name of the instance.

