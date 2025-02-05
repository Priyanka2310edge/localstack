# localstack

LocalStack
Localstack is a popular open-source project that enables developers to mimic various AWS services on their local development environments.
It provides a local alternative to AWS services, eliminating the need to make real requests to AWS during development and testing, thereby reducing costs and improving efficiency.

It's particularly useful for CI/CD pipelines, development environments, and testing scenarios where we want to avoid the overhead and potential issues of using live AWS services.
LocalStack can be run in Docker, and it supports a wide range of AWS services.

Docker:
LocalStack runs in a Docker container, so ensure we have Docker installed on our local machine.

AWS CLI:
Install the AWS CLI on our machine , it is require for configurations

Advantages of using localstack

1. offline development and testing.
2. CI/CD pipline intregation.
3. cost Efficiency.
   4.This speeds up the development cycle by allowing rapid testing and debugging.
   5.LocalStack also supports simulating AWS Lambda, making it useful for developers working on serverless applications that need to test Lambda functions locally before deploying to AWS.

Steps to install localstack on ubuntu

sudo apt update
sudo apt install docker.io -y

sudo systemctl enable docker –now
docker –version

To give access to user

sudo usermod -aG docker $USER
getent group docker
newgrp docker
sudo service docker restart

sudo apt install awscli
aws –version
pip install localstack==0.11.0
pip install dill==0.3.6
pip show localstack
