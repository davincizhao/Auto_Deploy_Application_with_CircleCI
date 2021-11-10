# Auto_Deploy_Application_with_CircleCI
CircleCI build pipeline on AWS with CloudFormation, deploy appliction backend and frontend in AWS, with AWS CLI,Ansible, Prometheus, AWS CLI,AIM


## Propose and Scope the Project
- CI/CD tool platform: CircleCI Cloud,AWS Cloudformation,AWS CLI, S3
- Application: NodeJS，NPM
- Repo: Github


## Tools
Tools:
- npm
- CircleCI
- AWS CLI, for AWS command line
- Ansible, for Config the backend server, configure prometheus and node-exporter in backend, deploy "backend artifact" and start npm。
- Prometheus,for monitoring the EC2 backend server.
![snapshot1](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT01.png)
![snapshot2](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT02.png)
![snapshot3](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT03.png)
![snapshot4](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT04.png)
![snapshot5](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT05.png)
![snapshot6](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT06.png)
![snapshot7](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT07.png)
![snapshot8](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT08.png)
![snapshot9](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT09.png)
![snapshot10](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT10.png)
### Prometheus,for monitoring the EC2 backend server
![snapshot11](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT11.png)
### Altermanger,for monitoring CI/CD pineline status, send alter message to slack
![snapshot12](https://github.com/davincizhao/Auto_Deploy_Application_with_CircleCI/blob/main/snapshot/SCREENSHOT12.png)
