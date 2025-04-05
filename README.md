# SIT323-2025-Prac5P - Containerisation of a Web App

## Overview

This project involves creating a simple web application using Node.js, Express, and Docker. The goal is to containerise the application using Docker and deploy it with Docker Compose.

## Technologies Used

- **Node.js**
- **Express**
- **Docker**
- **Docker Compose**

## Setup Instructions

### 1. Clone the Repository

To start, clone this repository to your local machine:

```bash
git clone https://github.com/yourusername/sit323-2025-prac5p.git
cd sit323-2025-prac5p

### 2. Install Dependencies

Run the following command to install the required dependencies:
```bash
npm install
```
### 3.Run the Application

To run the application locally without Docker:
```bash
node index.js
```
This will start the application on http://localhost:3000.

### 4. Docker Setup

If you want to run the application inside a Docker container, follow these steps:

#### 4.1 Build the Docker Image:

Run the following command to build the Docker image:
     
````bash
docker build -t my-cloud-app .
````
#### 4.2 Run the Docker Container:

Use the command below to run the container:

````bash
docker run -p 3000:3000 my-cloud-app
````
This will start the application inside the Docker container and map it to port 3000 on your local machine.

### 5.Docker Compose Setup
If you're using Docker Compose, you can use the following command to build and run the application:

```bash
docker-compose up --build
```
This will automatically build the image and start the container with the appropriate configurations.

### 6.Conclusion
This project demonstrates how to containerise a Node.js web application using Docker and Docker Compose for deployment.







