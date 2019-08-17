# iovio-task-five
##### status: *incomplete*

## Option 1: Verify the fastest and smallest algorithm for compression

## Option 2: Instantiate a computer in the cloud
### Pre-requisites (Windows with Docker Toolbox installed)
1. Windows with Docker Toolbox installed (No Hyper-V)
2. Docker service is running
## Steps to instantiate a virtual computer
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
