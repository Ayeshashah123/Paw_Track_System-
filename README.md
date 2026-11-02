# Paw_Track_System-
A team of Web developers, working on a Pet Adoption and Fostering System, named as Paw_Track

# Group Memebers
1. Urba Naseem - Group Leader
2. Shiza Shahid - Collaborator #01
3. Syeda Ayesha Fatima - Collaborator #02
4. Fasiha Tariq - Collaborator #03
5. Khansa Noor - Collaborator #04

# Deliverable - 1 
1. Created a basic home.html file
2. pushed on Git
3. Cloned by contributors
4. Contributors changes pushed to their respective branches
5. All the commits were merged into the main branch by the leader

# Deliverable - 2 (Building and Running  Docker Images)
1. Create a Docker file
2. Build the docker image
command : docker build --tag devops .
3. Run the docker image
command : docker run -d -p 8080:80 devops:latest  

# Deliverable - 3 (Added Backend Module and Created Docker-comper file)
1. Created Docker file for the Backend module
2. Created docker-compose.yml  
3. Application is run through the Docker compose

# Activity 2
Making changes in the README.md file to test the jenkins software 

# Change 2
Again just making minor change in the README file to generate build 2 in jenkins

# Deliverable - 4 (Automating CI/CD Pipeline)

This project demonstrates the implementation of an automated CI/CD pipeline using GitHub Actions and Docker.

CI/CD Pipeline
PawTrack uses GitHub Actions to automate Docker image building and deployment.

The pipeline automatically builds the Docker image whenever code is pushed to the main branch. The image is then pushed to Docker Hub.

Technologies Used:

GitHub

GitHub Actions

Docker

Docker Hub

AWS EC2 (optional deployment)

How to Run the Application

Build Docker Image

docker build -t .

Run Docker Container

docker run -d -p 8080:80 

Deployment

The application is deployed using Docker containers. GitHub Actions automates the build and image publishing process.

Changelog

Initial project setup

Added Docker support

Added GitHub Actions CI/CD workflow

Automated Docker Hub image publishing

Added deployment automation