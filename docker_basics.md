### Containerization and Orchestration Essentials

#### Description:

This project is designed to immerse students in the fundamentals of containerization and orchestration using Docker, Docker Compose, and GitHub Actions. Through a series of hands-on tasks, students will gain practical experience in creating, customizing, and deploying Docker images, managing data persistence, and orchestrating simple multi-service infrastructures. The project adopts a learn-by-doing approach, encouraging students to leverage provided resources, explore solutions independently, and collaborate to overcome challenges.

#### Objectives:

1. **Understanding Containerization:** Grasp the basics of containerization by creating and customizing Docker images based on the Alpine base image.
2. **Automating Workflows:** Learn how to automate the build and deployment of Docker images using GitHub Actions, fostering an understanding of CI/CD principles.
3. **Managing Data Persistence:** Explore the concept of data persistence in Docker by working with volumes to retain data across container restarts.
4. **Exploring Orchestration:** Dive into basic orchestration by setting up a simple infrastructure using Docker Compose, facilitating an understanding of multi-service deployments and inter-service communication.
5. **Applying Best Practices:** Implement best practices in Dockerfile creation, GitHub Actions workflow configuration, and Docker Compose setup to build a solid foundation for more complex projects.

### Resources:

- Familiarize yourself with Docker by going through the [Docker Official Documentation](https://docs.docker.com) and [Docker 101 Tutorial](https://www.docker.com/get-started).
- Learn about Docker Compose through the [Docker Compose Documentation](https://docs.docker.com/compose).
- Look into Docker image creation on [devopscube.com](https://devopscube.com/build-docker-image) and [linux.com](https://www.linux.com/learn/intro-to-linux/2018/1/how-create-docker-image).

---

## Task 1: Create a Simple Docker Image Locally Based on Alpine

#### Objective: 
Create a Docker image based on the Alpine base image that echoes "Hello, World!" when run.

#### Expected Output:
A Docker image that, when run, prints "Hello, World!" to the console.

---

## Task 2: Customize Your Alpine-based Docker Image

#### Objective: 
Extend your Docker image from Task 1 by adding the `curl` package and a configuration file named `config.txt` with the text "Welcome to Docker!".

#### Expected Output: 
A Docker image that, when run, can execute curl commands and where `config.txt` can be found with the specified text.

---

## Task 3: Automate Container Image Build and Push Using GitHub Actions

#### Objective: 
Set up a GitHub repository to hold your Dockerfile. Create a GitHub Actions workflow to build your Docker image and push it to the GitHub Container Registry whenever you push to your repository.

#### Expected Output: 
A GitHub Actions workflow that automatically builds and pushes your Docker image to the GitHub Container Registry upon each push to your repository.

---

## Task 4: Persist Data Using Volumes

#### Objective: 
Modify your Dockerfile to include a volume at `/data`. Demonstrate data persistence by writing data to the volume, then reading it back after stopping and restarting the container.

**Expected Output:** 
A demonstration showing data written to the volume is persisted across container restarts.

---

## Task 5: Set Up a Simple Infrastructure Using Docker Compose

#### Objective:

Create a Docker Compose YAML file to define two services: a web server and a database. The web server should serve a simple HTML page, and the database should be a simple key-value store like Redis. Ensure the web server can retrieve a value from the database and display it on the HTML page.

#### Expected Output:

A Docker Compose setup where the web server retrieves a value from the Redis database and displays it on the HTML page.

---

#### Challenge:

- Explore more complex setups with Docker Compose, such as adding more services, defining networks, and setting up dependencies between services.
- Look into other orchestration tools like Kubernetes and compare it with Docker Compose.
