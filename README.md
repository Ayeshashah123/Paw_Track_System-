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

This repository demonstrates a fully automated CI/CD pipeline using GitHub Actions. On every push to main or merge of a Pull Request, the pipeline automatically builds Docker images, pushes them to Docker Hub, and deploys the updated containers to an AWS EC2 instance via SSH.

Repository: AyeshaShah123/Paw_Track_System-

Docker Hub Repository: ayeshashah123/paw_track_system

AWS EC2 Target IP: 3.26.240.168

🔗 Live Application Endpoints

Frontend UI (Port 8081): http://3.26.240.168:8081

Backend API (Port 5000): http://3.26.240.168:5000

⚙️ CI/CD Pipeline Architecture (ci-cd.yml)

The pipeline defined in .github/workflows/ci-cd.yml executes two sequential jobs upon a push to main or a closed/merged pull_request:

┌────────────────────────┐      ┌────────────────────────┐      ┌────────────────────────┐
│  Git Push / PR Merge   │ ───> │     build-and-push     │ ───> │         deploy         │
│     (main branch)      │      │ (Builds & Pushes Hub)  │      │   (Deploys to EC2)     │
└────────────────────────┘      └────────────────────────┘      └────────────────────────┘
