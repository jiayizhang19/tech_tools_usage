## Dockerfile
See example Dockerfile.

## Image
### docker build --> build image based on Dockerfile
docker build -t cs50ai-app .

## Container
### docker run --> create container based on image
docker run -it --name cs50ai-container cs50ai-app /bin/bash
Note: remember to include /bin/bash in the command to enter bash, otherwise it will exit the container immediately after the current docker run command
### docker start --> re-enter the existing container 
docker start -ai cs50ai-container /bin/bash
### docker rename --> rename the container's name
docker rename previous_name cs50ai-container

### Git installation inside the container
#### Installation
apt-get update
apt-get install -y git
#### SSH 
ssh-keygen -t rsa -b 4096 -C "xxx@xx.com"
cat /root/.ssh/id_rsa.pub



