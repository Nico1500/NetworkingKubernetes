# Kubernetes Networking Overview

## Objective

This project is designed to test networking within a Kubernetes environment. By setting up 4 distinct pods, the project demonstrates how different services can interact securely within a Kubernetes cluster. The project components include a front-end user interface developed with React and three backend APIs: a User API, a Task API, and an Authentication API.

## Security

- The **Authentication API** is designed to be accessible only within the cluster (via Cluster IP), ensuring that authentication requests are secured and isolated from external access.

## Deployment

Components are deployed as pods within a Kubernetes cluster, providing isolation, resource management, and scalability.

## Networking

- **Internal Communication**: Services communicate with each other within the cluster via Kubernetes services like LoadBalancer and ClusterIP.
- **External Exposure**: The React frontend is made publicly accessible through a Kubernetes service of type LoadBalancer.
- **Security and Isolation**: The use of Cluster IP for the Authentication API ensures that the service remains private and inaccessible from outside the cluster.

## Technologies Used

- **Kubernetes** for container orchestration and networking.
- **React** for frontend development.
- **NodeJs** for the REST APIs and communication between the frontend and backend services.

## How It Works

Each folder contains its project and DockerFile to generate its image. The Kubernetes folder stores the yaml deployment and service files to use.

![image](https://github.com/Nico1500/NetworkingKubernetes/assets/63806892/0540dd78-ff31-493f-a20c-d250fc7830a0)
