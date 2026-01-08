# Containerized Web Application Deployment using Docker & AWS ECS (Fargate)

## Overview
This project demonstrates how to containerize a Python web application using Docker and deploy it on AWS ECS using Fargate. It covers the complete container lifecycle including image creation, pushing to Amazon ECR, ECS task execution, networking, and observability using CloudWatch.

## Architecture
- Python Flask application
- Docker for containerization
- Amazon ECR for image storage
- AWS ECS (Fargate) for container orchestration
- Custom Security Group for inbound traffic control
- Amazon CloudWatch for centralized logging

## Architecture Diagram

<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/177f6fe5-3b01-4f77-b438-2df70b44ca28" />

## Deployment Flow
1. Created a Dockerfile to containerize the Flask application
2. Built and tested the Docker image locally
3. Pushed the image to Amazon ECR
4. Created ECS Task Definition using Fargate
5. Deployed ECS Service with public IP
6. Configured custom security group and port mappings
7. Verified application accessibility and logs

## Observability
- Configured awslogs driver in ECS task definition
- Application logs streamed to CloudWatch log groups
- Enabled basic monitoring for container execution

## Security Considerations
- Used custom security group instead of default
- Allowed only required inbound ports
- IAM roles used for ECS task execution

## Screenshots
Refer to the screenshots folder for:

- ECS service running
  <img width="1906" height="817" alt="image" src="https://github.com/user-attachments/assets/dd56cc07-0d91-4160-8428-b5e49bd32f33" />
- Task networking details
  <img width="1631" height="559" alt="image" src="https://github.com/user-attachments/assets/007f3713-a726-4481-926a-496a9bc96892" />
  <img width="1640" height="411" alt="image" src="https://github.com/user-attachments/assets/6d55433d-06c2-4306-9511-3def9699849e" />
- CloudWatch logs
  <img width="1918" height="442" alt="image" src="https://github.com/user-attachments/assets/2d391f68-ee2c-42da-8baa-5b30a5243d4f" />
- Application output in browser
  <img width="936" height="329" alt="image" src="https://github.com/user-attachments/assets/1a9c860d-c04b-400a-b482-50b249259ea7" />

## Key Learnings
- ECS Fargate networking and port mappings
- Docker image lifecycle with ECR
- Importance of custom security groups
- Cloud-native observability practices

## Contact

- **Email:** [kunalshinde066@gmail.com](mailto:kunalshinde066@gmail.com)  
- **LinkedIn:** [Kunal Shinde](https://www.linkedin.com/in/kunal-shinde-1b17a2205)

---
