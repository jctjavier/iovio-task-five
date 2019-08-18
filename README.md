# iovio-task-five
##### status: *incomplete*

## Option 1: Verify the fastest and smallest algorithm for compression

## Option 2: Instantiate a computer in the cloud
### Pre-requisites (Windows with Docker Toolbox installed)
1. Windows/Linux/Unix with Docker installed
2. Docker service is running

## Steps to instantiate an EC2 instance in AWS
### Pre-requisites
1. AWS Credentials with an IAM administrator user
2. an AWS Access Key ID
3. an AWS Secret Access Key
### Steps
1. _(Optional)_ Create a credentials file in _~/.aws_ with the following information:
```
[default]
aws_access_key_id = AKID1234567890
aws_secret_access_key = MY-SECRET-KEY
```
2. Open a command shell
3. Run the following command:
a. With a credentials file:
```
docker-machine create --driver amazonec2 awsDefaultComputer
```
b. Without a credentials file:
```
docker-machine create --driver amazonec2 --amazonec2-access-key AKID1234567890 --amazonec2-secret-key MY-SECRET-KEY awsDefaultComputer
```
4. Run the following command to view instance details:
```
docker-machine ls
```
## Steps to instantiate a local virtual computer (For Windows with Docker toolbox installed. No Hyper-V)
1. Open a command shell
2. Run the following command: 
```
docker-machine create --driver virtualbox myDefaultComputer
```
where: 
--driver = indicate which provider we are using
virtualbox = since we are using an older Windows version with Docker toolbox, we will use virtualbox
myDefaultComputer = name of the instance
3. Run the following command to view instance details:
```
docker-machine ls
```
## Option 3: Write 5 lines of code in the Q programming language by KX systems
