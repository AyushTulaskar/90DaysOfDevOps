***Task 1:***


Introduction and Conceptual Understanding
Docker is an opensource centralised platform designed to create, deploy and run applications.
Docker uses container on the host os to run application it allows applications to use the some Linux kernal as a system on the best computer, rather than creating a whole vertual O.S.
Docker writen in 'go' Language
Docker is a tool that performs o.s. level virtualization also known as containerization.
Before Docker, many users faces the problem that a particular code is running in the developers system but not in the users system.

**Why is Docker Important in DevOps?**

Consistency: Docker ensures that your app works the same way everywhere—whether you're developing, testing, or deploying it. No more "it works on my machine but not on the server" problems!

Lightweight & Fast: Unlike traditional virtual machines (VMs), Docker containers share the host system's OS kernel, making them smaller, faster to start, and more efficient.

Scalability: Docker makes it easy to scale your app up or down based on demand, which is perfect for modern apps built with microservices (small, independent services).

CI/CD Integration: Docker fits seamlessly into CI/CD pipelines, automating the process of building, testing, and deploying apps. This speeds up software delivery and makes it more reliable.


**Virtualization vs. Containerization**

**Virtualization:**

Uses virtual machines (VMs) that include a full operating system.

Heavy on resources and slower to start.

Good for running different operating systems on the same hardware.

**Containerization:**

Uses containers that share the host OS kernel.

Lightweight, fast to start, and resource-efficient.

Perfect for microservices and CI/CD pipelines.

**Docker is Great for Microservices and CI/CD:**

Lightweight & Fast: Containers are small and start quickly, making them ideal for microservices (where you have many small, independent services).

Consistency: Docker ensures your app behaves the same way in every environment, reducing bugs and errors.

Scalability: You can easily scale individual microservices up or down as needed, saving resources.

Automation: Docker works well with CI/CD tools, automating the process of testing and deploying apps, which speeds up development.



***Task 2:***

Complited 



***Task 3:***

*Docker Image*:
A docker image is like a file that contains everything needed to run an application code, settings, dependencies.

*Docker Container*:
A Docker Container is like a small, portable box where an application runs along with everything it needs—code, libraries, and settings.
It ensures the application runs consistently on any computer, server, or cloud without worrying about differences in setup.

*DockerFile*:
A Dockerfile is like a recipe that tells Docker how to create a Docker Image.

It contains step-by-step instructions on:
What base image to use.
What software and dependencies to install.
What commands to run.
How to configure the application.

Docker reads the Dockerfile and builds a Docker Image, which can then be used to run containers.

*Volume*:
A Docker Volume is like a storage box that helps containers store and share data permanently.

By default, when a container stops, its data is lost. But with a Docker Volume, the data stays safe and can be reused, even if the container is restarted or deleted.

*Network*:
A Docker Network is like a communication system that allows Docker containers to talk to each other or the outside world.

By default, containers are isolated, but Docker Networks let them:
Connect and share data securely. Communicate with databases, APIs, or other services. Control traffic between containers 



*Main Docker Components & How They Interact*


 Docker Engine (The Core)
The main software that runs and manages containers. It listens to commands and handles everything from creating containers to networking and storage.

 Interaction: Receives commands via Docker CLI/API and executes them.

 Docker Image (The Blueprint)
The template used to create containers, containing all necessary files and configurations.

 Interaction: Pulled from Docker Hub or built using a Dockerfile.

 Docker Container (The Running Instance)
A live instance of an image, running an application in an isolated environment.

 Interaction: Created from Docker Images and managed by Docker Engine.

 Dockerfile (The Instruction Manual)
A script that automates the creation of Docker Images.

 Interaction: Used by Docker Engine to build Docker Images.

 Docker Hub (The Image Repository)
A cloud-based registry where Docker Images are stored and shared.

 Interaction: Users can pull images from Docker Hub or push their own images to share with others.

 Docker Volume (The Data Storage Box)
A persistent storage mechanism for saving data across container restarts.

 Interaction: Containers use volumes to store and retrieve important data.

 Docker Network (The Communication System)
A networking feature that allows containers to talk to each other or external services.

 Interaction: Containers use Docker networks to communicate securely.


***Task 4:***


A multi-stage build is a Docker technique that allows you to use multiple FROM statements in a Dockerfile to create an optimized final image. It helps in building an application in one stage and copying only the necessary files to the final stage, reducing image size.

Reduces Image Size:
Only the essential files are included in the final image.
Unnecessary build dependencies and tools are discarded.


Improves Security:
Removes sensitive files (e.g., API keys, build tools) from the final image.
Reduces attack surface by keeping the image lightweight.


***Task 6:***


**Why are Docker Volumes Useful?**

 Data Persistence – Prevents data loss when containers stop or restart.
 Easy Backup & Recovery – Volumes are stored separately, making them easy to back up.
 Container Independence – Multiple containers can share the same volume, ensuring data consistency.
 Improved Performance – Volumes are optimized for Docker and work faster than bind mounts.
