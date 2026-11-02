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

1. Description of CI/CD Pipeline
This project utilizes a GitHub Actions CI/CD pipeline configured at `.github/workflows/ci-cd.yml`. 
**Trigger**: The pipeline runs automatically when code is pushed to the `main` branch or when a pull request is merged.
**Build & Push:** It authenticates with Docker Hub using secure secrets, builds the frontend and backend Docker images, and pushes them directly to Docker Hub (`urbanaseem`).
**Deployment:** It securely connects to our AWS EC2 instance (`Jenkins-Server`) via SSH, pulls the updated images, and restarts the containers automatically[cite: 2].

2. Instructions to Run and Deploy the App
**Local Run using Docker Compose:**
  docker-compose up --build -d
**Run Containers Manually from Docker Hub:**
  docker pull urbanaseem/paw-track-backend:latest
  docker pull urbanaseem/paw-track-frontend:latest
  docker run -d --name paw-backend -p 5000:5000 urbanaseem/paw-track-backend:latest
  docker run -d --name paw-frontend -p 80:80 urbanaseem/paw-track-frontend:latest