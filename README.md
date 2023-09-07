# Cloud-Native Web Voting Application with Kubernetes

## Table of Contents
1. [Introduction](#introduction)
2. [Technical Stack](#technical-stack)
3. [Kubernetes Resources](#kubernetes-resources)
4. [Learning Opportunities](#learning-opportunities)
5. [Project Architecture](#project-architecture)
6. [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Deployment Steps](#deployment-steps)
7. [Final Deployment](#final-deployment)
8. [Acknowledgments](#acknowledgments)

## Introduction

A scalable and cloud-native web application built on Kubernetes, allowing users to vote for their favorite programming languages. The languages include C#, Python, JavaScript, Go, Java, and NodeJS.

## Technical Stack

- **Frontend**: React, JavaScript
- **Backend**: Go (Golang) serves as the API handling user voting requests
- **Database**: MongoDB with Replica Set for High Availability

## Kubernetes Resources

This application leverages several Kubernetes resources for optimal deployment and management:

- Namespace
- Secret
- Deployment
- Service
- StatefulSet
- PersistentVolume & PersistentVolumeClaim

## Learning Opportunities

By working on this project, you will gain hands-on experience in:

- Containerization with Docker
- Kubernetes Orchestration
- Microservices Architecture
- Database Replication
- Security and Secrets Management
- Stateful Applications
- Persistent Storage

## Project Architecture

![three tier cloud native architecture](https://github.com/prajwalpd7/KubeVote-EKS-Edition/assets/71492927/6a23ce2b-6c41-49aa-8a83-caec65e7a681)

## Getting Started

### Prerequisites

- Kubernetes Cluster (EKS)
- kubectl
- AWS CLI

### Deployment Steps

1. **Clone this Repository**:  
   `git clone https://github.com/prajwalpd7/KubeVote-EKS-Edition`

2. **Setup MongoDB**:  
   Run the commands inside the manifests folder:  
   `kubectl apply -f mongo-statefulset.yaml`  
   `kubectl apply -f mongo-service.yaml`

3. **API Setup**:  
   Create the API deployment:  
   `kubectl apply -f api-deployment.yaml`

4. **Frontend Setup**:  
   Create the Frontend deployment:  
   `kubectl apply -f frontend-deployment.yaml`

For detailed steps, follow this [repo](https://github.com/N4si/K8s-voting-app).

## Final Deployment

![Screenshot (70)](https://github.com/prajwalpd7/KubeVote-EKS-Edition/assets/71492927/9fb3377e-6657-4c08-a905-dca37036411e)



![Screenshot (69)](https://github.com/prajwalpd7/KubeVote-EKS-Edition/assets/71492927/7304707b-f55f-448a-9025-64fdf7fabf40)

## Acknowledgments

- Open Source Community
- Kubernetes and Docker
- Anyone who contributes to this project

---
