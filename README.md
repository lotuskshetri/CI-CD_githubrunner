# CI-CD_githubrunner
This repo is solely for the documentation related to task 1 to be assessed by GlobalyHub

Task-1 : Write CI/CD Deployment Task Using GitHub Runner

1. Server setup (write bash script):
   
a. A virtual machine was creaated in VMware Workstation with ubuntu-24.04.2-live-server-amd64.iso.     Openn SSH service was also installed and intialized for remote access outside the VM.

b. server-setup.sh was creaeted to reinstall docker and install nginx and enable its services
Dokcer was reinstalled through "sudo apt install -y docker.io" after the docker was found not be enabled.

c. Both docker and nginx were found to be running after executing status check

d. An example react project was uploaded to the repo git@github.com:lotuskshetri/reactappexample.git which will act as our sample project for CI/CD.

e. SSH key for the ubuntu server was added to the github for future ease.

f. Dependencies were installed and docker image was created.

1.2 After getting access to EC2 same process was repeated.

a. The image pushed in dockerhub was pulled in the server 

b. Docker composer.yml was also created

c. Repositories secrets were added in actions

d. cicd.yml was created for CD that triggers build in github actions after commits in repositories were detected.

e. This concludes the CI/CD cycle.
 

