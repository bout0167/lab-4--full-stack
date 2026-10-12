# Lab 4: CST8915 Full-stack Cloud-native Development: Introduction to Docker

[Demo link](https://youtu.be/cnTEyzH-6EY)

## 1. What are the main differences between a Docker image and a Docker container?
A Docker image is a file that contains everything needed to run an application. A container is created from an image and runs the application. Many containers can use the same image.

## 2. Explain how Docker's layered architecture improves efficiency.
Docker images have different layers that can be reused. When something changes, Docker only needs to rebuild the changed layers instead of rebuilding everything. This saves time and storage space.

## 3. Why does each container get its own writable layer?
Each container has its own writable layer to save its changes. This means changes in one container do not affect other containers or the original image. The changes are lost when the container is deleted.

## 4. What are the benefits of using Docker Compose over running containers individually?
Docker Compose makes it easier to manage multiple containers. It uses one file to define the containers and how they work together. We can start, stop, and manage all the containers with simple commands instead of managing each one separately.