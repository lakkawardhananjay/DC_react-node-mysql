# DC React-Node-MySQL Web Application

This project is a full-stack web application that uses **React** for the frontend, **Node.js** for the backend, and **MySQL** as the database. It demonstrates a modern development approach, integrating these technologies .

## Project Overview

The **DC_react-node-mysql** project integrates a responsive React frontend with a Node.js backend, powered by a MySQL database. The application showcases basic  functionalities, allowing seamless interaction between the frontend and backend through REST APIs.

## Technologies Used
- **Frontend**: React
- **Backend**: Node.js, Express.js
- **Database**: MySQL

## Prerequisites
To run the application, ensure you have the following installed on your machine:
- Node.js (v14 or higher)
- MySQL
- npm (Node Package Manager)
- Docker Desktop
- Doceker compose

## Installation Instructions

### 1. Clone the Repository:
```bash
git clone https://github.com/lakkawardhananjay/DC_react-node-mysql.git

````

### 2. **Provisioning the EC2 Instance**

- Go to the **AWS Management Console** and launch an EC2 instance.
- Select an **Ubuntu** image (or another Linux flavor).
- Configure the security group for the EC2 instance:
  - **Port 80** (HTTP) for web traffic.
  - **Port 443** (HTTPS) for secure traffic.
  - **Port 22** (SSH) for remote access.

### 3. **Install Docker, Docker Compose, and NPM**

Once the EC2 instance is launched, SSH into it and run the following commands:

```bash
# Update the package list
sudo apt-get update

# Install Docker
sudo apt-get install -y docker.io

# Install Docker Compose
sudo curl -L "https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

# Add the user to the Docker group to avoid using sudo with Docker
sudo usermod -aG docker $USER

# Install Node.js and NPM
sudo apt-get install -y nodejs npm
```
### 3. Clone the GitHub Repository
Once Docker and NPM are installed, clone the application repository from GitHub to the EC2 instance :
```bash
git clone https://github.com/lakkawardhananjay/DC_react-node-mysql.git
```
###4. Running Docker Compose Manually
To ensure everything works as expected, you can manually run Docker Compose on the EC2 instance.
```bash
docker-compose up  --build
```
🎉 Joyful Note!
With these steps, you can effortlessly run the application! 🎊 Enjoy the seamless deployment of your 3-tier application on AWS EC2. Happy coding and may your app thrive! 🚀✨
