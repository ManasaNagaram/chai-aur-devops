# Chai Code DevOps Assignment

## Assignment Description

The provided repository contains a basic full-stack application with the following components:

1. A basic Express.js server with basic & courses endpoint
2. A React.js frontend application
3. Redis integration for API response caching
4. MongoDB integration for data storage

## Objective

Your task is to containerize the application for a "Development" environment using Docker. Ensure that all components work seamlessly together within their respective containers and work as per the provided screenshots below.

## Note

The application environment variables are stored in a `.env` file. You can find the `.env.example` file in the respective directory. Copy it to `.env` and fill in the required values.

## Screenshots

### Home Page

![Screenshot 1](./screenshots/One.png)

### Load Data from MongoDB

![Screenshot 2](./screenshots/Two.png)

### API Response Caching

![Screenshot 3](./screenshots/Three.png)


---



### 1. Clone the Repository

```bash
git clone https://github.com/ManasaNagaram/chai-aur-devops
cd chai-aur-devops
## create .env file 
```
### 2. Start All Services with Docker Compose

```bash
docker-compose up -d
```
or pass environment variables
```bash
$env:PORT="8000"
$env:REDIS_PASSWORD="mypass"
docker-compose up -d
```
3. Seed MongoDB with Initial Data
```bash
docker exec -it backend node seed.js
```
Access app at:

http://localhost:5173

