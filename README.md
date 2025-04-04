# USVisa-Approval

- Anaconda: https://www.anaconda.com/
- Vs code: https://code.visualstudio.com/download
- Git: https://git-scm.com/
- FlowChart: https://whirmsical.com/
- MLOPs Tool: https://www.evidentlyai.com/
- MongoDB: https://account.mongodb.com/account/login
- Data Link: https://www.kaggle.com/datasets/moro23/easyvisa-dataset

## Git commands

```cmd
git add .

git commit -m "Updated"

git push origin main
```

```cmd
conda create -n visa python=3.9 -y
```

```cmd
conda activate visa
```

```cmd
pip install -r requirments.txt
```


## Workflow:               
1. constants
2. entity
3. components
4. pipeline
5. Main file


# s3

# Save the keys in local Machine Env if using windows 

- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY


# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console.

## 2. Create IAM user for deployment

     #with specific access

     1. EC2 access : It is virtual machine

     2. ECR: Elastic Container registry to save your docker image in aws


     #Description: About the deployment

     1. Build docker image of the source code

     2. Push your docker image to ECR

     3. Launch Your EC2 

   a  4. Pull Your image from ECR in EC2
 
     5. Lauch your docker image in EC2

     #Policy:

     1. AmazonEC2ContainerRegistryFullAccess

     2. AmazonEC2FullAccess

## 3. Create ECR repo to store/save docker image

     - save the ECR URI: 

# 4. Create EC2 machine (Ubuntu)

# 5. Open EC2 and Install docker in EC2 Machine:

     #optinal

     sudo apt-get update -y

     sudo apt-get upgrade

     #required

     curl -fsSL https://get.docker.com -o get-docker.sh

     sudo sh get-docker.sh

     sudo usermod -aG docker ubuntu

     newgrp docker

# 6. Configure EC2 as self-hosted runner:

     setting>actions>runner>new self hosted runner> choose os> then run command one by one

# 7. Setup github secrets:

- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
- AWS_DEFAULT_REGION
- ECR_REPO
