 

# Deploy an App with Docker
  ##   Abhinav Singh



![image](https://github.com/animatorsingh/awsBeanStalk/blob/7babc43f3a4b564f534045211955911d3d1a1f36/Images/Screenshot%202025-09-09%20131721.png)

 

Introducing Today's Project!
What is Docker?
Docker is is a tool which helps you to contanarized your application and its useful because then you dont have to worry about os version and about dependencies of your application


One thing I didn't expect...
One thing I didn't expect in this project was it going to be so easy


This project took me...
This project took me approximately 30 mins
 

Understanding Containers and Docker

Containers
Containers package up your application and everything it needs to run (i.e. dependencies) in one file. Now other developers can run this package instead of the application itself, which gets the application working much faster.


A container image is which your dependencies and all other stuff is pre defined to run you appliation or how to run your application


Docker
Docker is a tool create and update images and container Docker Desktop is a ui interface of this tool to so user can work on this easily


The Docker daemon is the engine that actually □ does the thing □ when you run Docker commands e.g. create a container
 

Running an Nginx Image

Nginx is a web server ,which is a program you use to run websites and web apps. If you want people to visit your site, you're going to need a web server to deliver your website's files to their browsers!


The command I ran to start a new container was docker run -d -p 80:80 nginx
 

Creating a Custom Image

The Dockerfile is a pre set rules in which type steps how to build docker image


My Dockerfile tells Docker three things are first install nginx server then in
/usr/share/nginx/html/ copy index.html file and at last it says to expose port 80


The command I used to build a custom image with my Dockerfile was docker build -t my-web-app . The '.' at the end of the command tells Docker to find the Dockerfile in the current directory i.e. the Compute folder
 

Running My Custom Image

There was an error when I ran my custom image because... I resolved this by removing earlier container


In this example, the container image is where all steps and depencies are written how to run my application, and the container is where my applicaiton actually runs
 

Elastic Beanstalk

AWS Elastic Beanstalk is a service that makes it easy to deploy cloud applications without worrying about the underlying infrastructure. You simply upload your code and Elastic Beanstalk handles everything needed to get it running, like setting up se


Deploying my custom image with Elastic Beanstalk took me around 15 mins
 













