**Deploying a Node Js Application on AWS EC2**

1. Clone this project:

https://github.com/Abhishek-Sontakke/My_React_Project.git

2. Initialise and start the project
 
* npm install
* npm run start
  
3. Set up an AWS EC2 instance

3.1 Create an IAM user & login to your AWS Console
 * Access Type - Password
 * Permissions - Admin

3.2 Create an EC2 instance
* Select an OS image - Ubuntu
* Create a new key pair & download .pem file
* Instance type - t2.micro
 
3.3 Connecting to the instance using ssh:

ssh -i instance.pem ubunutu@<IP_ADDRESS>


4. Configuring Ubuntu on remote VM

 4.1 Updating the outdated packages and dependencies:
 
  sudo apt update

4.2 Install Git - Guide by DigitalOcean
4.3 Configure Node.js and npm - Guide by DigitalOcean

**Deploying the project on AWS**

1. Clone this project in the remote VM
https://github.com/Abhishek-Sontakke/My_React_Project.git

2. Initialise and start the project
 
* npm install
* npm run start
 

 * NOTE - We will have to edit the inbound rules in the security group of our EC2, in order to allow traffic from our particular port

Project is deployed on AWS 🎉
