# AWS-CICD-Website-Deployment
This project automates website deployment using AWS services like CodePipeline, CodeDeploy, CodeCommit, S3, and EC2. The goal was to create a seamless CI/CD pipeline for automating integration, build, and deployment to host a live website.
Streamlined Web Deployment: Building a CICD Pipeline with AWS CodePipeline and CodeDeploy
Project Overview:-
This project demonstrates an end-to-end automated website deployment using AWS services such as CodePipeline, CodeDeploy, CodeCommit, S3, and EC2. The goal was to build a seamless CI/CD pipeline to automate integration, build, and deployment processes for hosting a live website.
Key Features:-
1)IAM Roles and Permissions: Configured roles for EC2 and CodeDeploy to enable secure access.
2_S3 Storage: Used for storing build artifacts.
3)CodeCommit: Repository for managing and version-controlling code.
4)CodeBuild: Automates packaging and builds the application.
5)CodeDeploy: Manages deployment to EC2 with custom lifecycle hooks.
6)CodePipeline: Integrates all steps (Source → Build → Deploy) into a streamlined CI/CD workflow.
Technologies Used:-
1)AWS CodePipeline
2)AWS CodeDeploy
3)AWS S3
4)AWS EC2
5)AWS IAM
6)AWS CodeBuild
7)Git
Setup and Workflow
Steps to Recreate the Project
1]Create IAM User and Roles:
Configure roles for EC2 and CodeDeploy with appropriate policies.
2]Launch EC2 Instance:
Use an Ubuntu AMI and attach the EC2 role.
Ensure the CodeDeploy agent is installed and active.
3]Set Up S3 Bucket:
Create a bucket to store build artifacts.
4]Create a CodeCommit Repository:
Clone the repository locally using Git.
Upload project files using Git commands.
5]Configure CodeBuild:
Create a build project and use a buildspec.yml file.
6]Set Up CodeDeploy:
Create a deployment group and define lifecycle hooks using appspec.yml.
7]Integrate into CodePipeline:
Define stages for source (CodeCommit), build (CodeBuild), and deploy (CodeDeploy).
8]Test Deployment:
Access the website via the EC2 public IP in your browser.
Key Learnings
1]Practical understanding of CI/CD pipelines using AWS services.
2]Configuring and integrating multiple AWS tools for automated workflows.
3]Debugging deployment issues with lifecycle hooks and IAM policies.
