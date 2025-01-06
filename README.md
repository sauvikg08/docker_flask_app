# Simple Python App Deployed with Flask and Docker
This project demonstrates a basic Python application built with the Flask framework, which displays "Hello World" when accessed. The application is containerized using Docker for easy deployment and portability.

Features
A minimal Flask application serving a "Hello World" response.
Environment setup and deployment using Docker.
Lightweight and easy to extend for learning or small-scale projects.
Prerequisites
Before running this project, ensure you have the following installed:
```
Python 3.8+
Docker
```

Project Structure

```
├── app.py               # Flask application
├── Dockerfile           # Docker configuration
├── requirements.txt     # Python dependencies
```
Usage
1. Build the Docker Image
Run the following command to build the Docker image:

```
docker build -t welcome-app .
```
2. Run the Docker Container
Run the container using:

```
docker run -p 5000:5000 welcome-app
```
3. The Docker Image has been renamed based on standard naming techniques

```
docker tag welcome-app aspiringai/welcome-app
```
# Renaming and Pushing to Docker Hub
4. Access the Application

Visit http://localhost:5000 in your browser or use a tool like curl:

```
curl http://localhost:5000
```
You should see:

```
Hello World
```
5. Docker file pushed to docker hub using:

```
docker push aspiringai/welcome-app:latest
```

6. Extending the Application
The application can be extended by 
* Adding more routes and functionality.
* Integrating a database for dynamic data handling.
* Deploying the containerized application to a cloud platform (e.g., AWS, Azure, or GCP).