# Overview
This repository contains a React frontend, and an Express backend that the frontend connects to.

# Objective
Deploy the frontend and backend to somewhere publicly accessible over the internet. The AWS Free Tier should be more than sufficient to run this project, but you may use any platform and tooling you'd like for your solution.

Fork this repo as a base. You may change any code in this repository to suit the infrastructure you build in this code challenge.

# Submission
1. A github repo that has been forked from this repo with all your code.
2. Modify this README file with instructions for:
* Any tools needed to deploy your infrastructure
* All the steps needed to repeat your deployment process
* URLs to the your deployed frontend.

# Tools Needed
1. A working AWS account
2. Code Editor
3. [Node](https://nodejs.org/en/download/)
4. Docker
5. Docker Compose

For Docker and Docker Compose the file [setup.sh]() canbe used for installation and [run.sh]() can be used to run docker compose, use:
```
bash setup.sh
```

# Steps
1. Create IAM ROle for EC2 and CodeDeploy
2. Create EC2 instance and attach the role created
3. Remote into instance
4. Install CodeDeploy Agent on Instance
5. Configure DodeDeploy and attach the role created in step 1
6. Visit <ec2_public_ip:port>
7. Update repository settings by adding secrets such a AWS_ACCESS_KEY, AWS_REGION, AWS_SECRET_KEY
8. Create Github Action workflow
9. Push to repository

# Steps to run locally
1. use the command 
```
docker-compose up
```
2. For the frontend visit 
```
localhost:3000
```

The Backend and FrontEnd of the application is hosted in AWS
[Backend](52.79.177.178:8080)
[Frontend](52.79.177.178:3000)