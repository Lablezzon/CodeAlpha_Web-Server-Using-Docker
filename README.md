# CodeAlpha_Web-Server-Using-Docker

# 🚀 Docker Web Server Deployment (NGINX)

## 📌 Project Overview
This project demonstrates how to deploy a simple web server using Docker. It uses an NGINX container to serve a custom HTML webpage from a Docker image built using a Dockerfile.

The goal of this project was to understand Docker containerization, image building, and running a web server inside a container.

---

## 🛠️ Tools & Technologies Used
- Docker Desktop
- NGINX Web Server
- HTML
- Windows OS
- Dockerfile

---

## 📁 Project Structure

docker-web/
│
├── Dockerfile
└── index.html


---

## ⚙️ How It Works

1. A simple `index.html` file was created.
2. A `Dockerfile` was written to:
   - Use the official NGINX image
   - Copy the HTML file into the NGINX web directory
3. A Docker image was built using the Dockerfile.
4. A container was created from the image.
5. The web server was accessed via browser.

---

## 🐳 Dockerfile Used

dockerfile
FROM nginx
COPY index.html /usr/share/nginx/html/index.html


🚀 Steps to Run the Project
1. Build Docker Image
docker build -t mywebsite .


<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/41452bd2-b0f9-4d0c-8f26-553b11d61388" />

3. Run Container
docker run -d -p 8080:80 --name my-site mywebsite
4. Access Web Server

Open browser and visit:

http://localhost:8080

🌐 Expected Output

A simple webpage displaying:
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/83c6a7ce-3aef-43da-a49f-8d56d08af25d" />


Docker is Working Successfully!
This web server is running inside a Docker container.


📚 What I Learned

Basics of Docker containerization

Creating and managing Docker images

Writing a Dockerfile

Running NGINX inside a container

Port mapping in Docker

Deploying a simple web server using containers

🔥 Key Commands Used

docker build
docker run
docker ps
docker stop
docker rm

📌 Author

Blessing Taiwo
GitHub: (https://github.com/Lablezzon)
