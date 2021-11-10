# Auto_Deploy_Application_with_CircleCI
CircleCI build pipeline on AWS with CloudFormation, deploy appliction backend and frontend in AWS, with AWS CLI,Ansible, Prometheus, AWS CLI,AIM

## Pre-requirement
Login in CircleCI.com and connect your github with circleci.
- 1. select project that you want to work in CircleCI, and press "Set Up Project"
- 2. create new config.yaml or choose from repos ".circleci/config.yaml"

## Propose and Scope the Project
- CI/CD tool platform: CircleCI Cloud,AWS Cloudformation,AWS CLI, AWS EC2, AWS S3,AWS Cloudfront
- Config tool: Ansible
- Monitoring: Prometheus, Altermanager
- Application: NodeJS，NPM
- Repo: Github


## Tools
Tools:
- NPM, package manager for the JavaScript
- CircleCI
- AWS CLI, for AWS command line
- Ansible, for Config the backend server, configure prometheus and node-exporter in backend, deploy "backend artifact" and start npm。
- Prometheus,for monitoring the EC2 backend server.
### 1 Build Backend node.js code and find out the error, troubleshooting in build Stage.
![snapshot1](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT01.png)
### 2 Atfer build, Test backend and find out error, troubleshooting.
![snapshot2](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT02.png)
### 3 Build Frontend code and find out the error, Scan front-end dependencies, troubleshooting in build Stage.
![snapshot3](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT03.png)
### 4 Auto send alter to email, when there's fail job or step in CircleCI pipeline. 
![snapshot4](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT04.png)
### 5 Deploy infrastructure (frontend and backend), aws cli,aws cloudformation, etract back-end ip to ansible inventory,Test infrastructure, ensure the backend infrastructure exist
![snapshot5](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT05.png)
### 6 After Deploy, Smoke test both frontend and backend
![snapshot6](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT06.png)
### 7 Smoke test, if there's error, auto destroy enviroments(cloudformation stacks with workflow ID) in AWS and revert migrations.
![snapshot7](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT07.png)
### 8 Smoke test is ok, now Update cloudfront distribution.
![snapshot8](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT08.png)
### 9 Clear up, Remove old stacks and S3 files in AWS 
![snapshot9](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT09.png)
### 10 According to different github branch, run specify jobs, like in build stage, only run "build and test" job in CircleCI
![snapshot10](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT10.png)
### 11 Prometheus: EC2 server in AWS connected to prometheus server
![snapshot11](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT11.png)
### 12 Altermanger,for monitoring backend server status in AWS, auto send alter messages to slack
![snapshot12](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT12.png)
