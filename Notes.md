# Docker
![image](https://github.com/user-attachments/assets/e14c7238-9d0d-488b-b568-c63cafa7cba6)  

![image](https://github.com/user-attachments/assets/d043c43d-b877-4e1a-b392-9f1e0d741727)  

![image](https://github.com/user-attachments/assets/b2c6cb61-7a43-486e-b425-460fcb44235d)  

![image](https://github.com/user-attachments/assets/b79b8f00-6c0b-43ea-aada-dffe28986822)  

![image](https://github.com/user-attachments/assets/1d500594-220f-4f2d-8b90-b11e3506f083)  

![image](https://github.com/user-attachments/assets/14f7d41c-a900-441b-ae38-db4db09dd096)  

![image](https://github.com/user-attachments/assets/72538cb3-38c6-4c87-aa6e-c3d26a4f5b7d)  

![image](https://github.com/user-attachments/assets/558c1f9d-0e2a-4577-a0fe-a569270673c1)  

![image](https://github.com/user-attachments/assets/b0fdbd95-57b9-4287-8a8e-5f226f2fd5c9)  

![image](https://github.com/user-attachments/assets/e2c65179-ed14-4533-9f07-d438bce4bef7)  

![image](https://github.com/user-attachments/assets/4483fa58-aa77-44f4-90b7-591fa7106225)

## What is docker?
Docker is a virtualization software. It makes development and deploying applications much easier. 
Docker packages the application into a container that has everything an application needs to run. 
This includes the application code, its libraries, dependencies, and the run-time environment such as node.js and environment configurations. 
So, an application and the run-time environment are packaged together in a single docker package. This can be easily shared and distributed.  
![image](https://github.com/user-attachments/assets/19ac59b8-1f4b-4d86-b9e8-bd4962ca46f8)  

## What problems are solved by docker?
### Development process before containers
![image](https://github.com/user-attachments/assets/f364e69a-52fa-47a3-a929-418aad2315e4)  

Whatever application you are developing, you will have to install all the needed software for that and also you have to do the configurations for those. 
All the developers on the team will have to do the same. 


![image](https://github.com/user-attachments/assets/27654b83-8458-48c3-9d21-ebdc91d913ab)  

![image](https://github.com/user-attachments/assets/cde9d19f-3e75-4380-9202-4d2f7ee8d06e)  

### How do containers solve these problems?
No need to install any services or software directly on your local machines. 
With containers/docker, the service is packaged in an isolated env.
For example, PostgreSQL with a specific version and specific configurations is packaged inside a container. 
Now, you can start this service(here it is PostgreSQL) as a docker container with a single docker command. 
This command will fetch the container from the internet and start it on your computer. 
The Docker command is the same for all the operating systems.  

![image](https://github.com/user-attachments/assets/75044e5d-ad71-4a86-b75a-36d293f227b9)  

The docker command also remains the same regardless of which service you want to use. 
For example, if your app has ten services that it depends on, you will have to use ten docker commands for ten containers.  

![image](https://github.com/user-attachments/assets/48aff7b6-7072-4135-b1f7-0edffe52bcc5)  ]

With docker, the process of running any service on your local machine is standardized. Installing and configuring a service becomes easy. 
More time for development.  

![image](https://github.com/user-attachments/assets/f39a880e-df34-42e2-8a0c-fb0a04c6ed95)  

It is also easy to run different versions of the same application on your local environment.  

![image](https://github.com/user-attachments/assets/e181df6b-63f9-459e-afe4-87f29effa35c)  

### Deployment process before containers
The development team will produce an artifact or a package such as a .jar file in the case of Java. They will also provide instructions on how to install and configure the package on the server.
If your application is also using some database service, those have to be installed on the server as well.  
Dev teams will give those artifacts to the ops team. The ops team will install and configure everything on the server as per the instructions given by the dev team.  

![image](https://github.com/user-attachments/assets/0babf554-0740-44ac-b3b0-57cede6247fc)  

Problems:
![image](https://github.com/user-attachments/assets/1713eb0a-88ac-497b-b067-d1e0ae7861ba)  

![image](https://github.com/user-attachments/assets/e0f99531-6b0c-43dc-8fe9-3eb72106c75b)  

![image](https://github.com/user-attachments/assets/f98d36bc-36e3-4a72-914c-fcd4c40ae487)  

![image](https://github.com/user-attachments/assets/e1b3908c-71c6-45b8-a010-e975a0ee12b6)  

### How do containers solve these problems?
Now, the developers create an application package that does not include the code itself but also all the dependencies and all the configurations for the applicaiton.  

![image](https://github.com/user-attachments/assets/d15a8d11-4e87-4fde-97f2-d0cdfdfd9023)  

Instead of an instructions document, they will package it inside the application artifact.  

![image](https://github.com/user-attachments/assets/5593680f-4ef0-4d1e-9889-bbb95f29b385)  

1. No configurations needed to be done on the server directly by the ops team.
2. Less room for errors.
   
The Ops team now only has to do the following tasks:
1. Run the command to get the docker package created by the dev team.
2. Run  this package on the server.

![image](https://github.com/user-attachments/assets/7a1f2294-b528-4a34-bc24-933ff2ed71e4)  

## VMs vs Docker
![image](https://github.com/user-attachments/assets/fe8b4766-7095-479b-82d4-0a2f681ef1f7)  

![image](https://github.com/user-attachments/assets/93cbc014-e20d-4f61-bdfd-9c8ecec91080)  

### Understanding how OS works
![image](https://github.com/user-attachments/assets/493cb678-bcc9-497c-a345-11c3f60a0a3c)  

### Virtualization
Docker virtualizes the application layer of the OS. When you run the docker container, it contains the OS application layer.  
It uses the kernal of the host OS because it does not have its own kernal.  
VM virtualizes the kernal and the application layer of the OS. So, the complete OS.  
![image](https://github.com/user-attachments/assets/733812f3-a184-4da5-90e9-3eab44c644fe)  

![image](https://github.com/user-attachments/assets/eece852e-238e-4cbb-a7b0-97edb0fcde61)  

### Difference
The size of the docker image will be much smaller.  
Boot time for a docker image is much smaller than a VM. 
VMs are compatible with any OS. On a Windows machine, you can run a Linux VM with no issues.  

![image](https://github.com/user-attachments/assets/ebae10ba-199b-4590-9b9e-02d96af53339)  

Why a docker image can only run on the Linux OS?
Docker will use the kernal of the host OS. If the host OS is Windows then the docker Linux image cannot use it, since it will need a Linux kernal.  

![image](https://github.com/user-attachments/assets/53735c8b-aa1e-40f9-b6ac-7fe8cf9d7431)  

**Most docker containers are Linux-based.**  
**We need to use docker desktop to use docker on Windows and MacOS.**  
**Docker desktop uses a hypervisor layer with a lightweight Linux distro.**  

## Docker Installation
### Installing Docker Desktop
![image](https://github.com/user-attachments/assets/d7a78736-2414-4789-a2d1-270222b36394)  

![image](https://github.com/user-attachments/assets/f6cd81d2-3e9e-44c8-9638-1468fe54a36c)  

## Docker Images vs Docker Containers
### Docker Image
Docker allows to package an application with its env configs into a package.  

![image](https://github.com/user-attachments/assets/d607423a-3441-4d96-8ae4-fa4a3af8127d)  

This package can be shared and distributed easily. This package is called **Docker Image**.  

![image](https://github.com/user-attachments/assets/87d4120d-7ca5-4085-8189-d56d0d3eb2db)  

A docker image will have:  
1. Complied application code
2. Operating system application layer(not the OS kernal)
3. Any tools needed to run the application such as node, npm, etc.
4. Environment variables, directories, files, or any other env configs you need to run the application.

![image](https://github.com/user-attachments/assets/73697fd3-e7a7-40cf-acb4-ec56be6cefd2)  

### Docker Container
We need to start/run the docker image somewhere, right? 
The docker image will run in a pre-configured environment. This will be the docker container.  
The running instance of a docker image is a docker container.  
![image](https://github.com/user-attachments/assets/02368309-9812-477f-876d-5d89a5eef07b)  

![image](https://github.com/user-attachments/assets/c2eb7ea2-fc44-4abc-a27e-c6874a024d82)  

You can run multiple containers with the same image.  
![image](https://github.com/user-attachments/assets/0a3bcffa-9df3-4c5c-b28f-a37f8d495923)  

This is a use case when you need to run multiple instances of your application. This can be due to high traffic.  
First, create the image and then run that image in a docker container.  

## Docker UI on Windows
### Docker Home Page
![image](https://github.com/user-attachments/assets/19ffa856-231e-4f32-9385-184caddc1087)  

### Docker Terminal
![image](https://github.com/user-attachments/assets/3a1290ac-a95a-47c7-86f9-5566795a0c1e)  

### Basic Commands
![image](https://github.com/user-attachments/assets/6aea5f32-a578-4811-96ec-7a75dcfbe7ff)  

![image](https://github.com/user-attachments/assets/a63d08db-4ffe-4c3d-84a1-bcb239fc8747)  

## Docker Registry
### How do we get docker images?
Let's say we want to run a database container or Redis or some other service. This is where we use docker registries. 
The Docker registry will have ready Docker images available online in an image storage or registry storage.  
![image](https://github.com/user-attachments/assets/0c7245dc-05b9-4647-85d6-64948213734f)  

You can get docker images for applications such as Redis, Mongo, Postgres, etc. These are official images created by official companies.  
![image](https://github.com/user-attachments/assets/524e656b-f5fe-4e2e-9a75-bafc360a94b3)  

Docker hosts one of the biggest Docker registry called **Docker Hub**.  
![image](https://github.com/user-attachments/assets/0894ea5c-6a08-4f2e-8548-adae8d3fac7d)  


![image](https://github.com/user-attachments/assets/2a82217d-9f0d-47f3-bd67-d126a11f4d57)  

### How does docker image versioning work?
Docker images are versioned. 
When we have a new version of the application, a new version of the image is also released.  

![image](https://github.com/user-attachments/assets/a2eb5d33-6e00-487f-8c04-11b3262f8df0)



Images are versioned. Versions are called image tags.  
Here is the Redis image page on the docker hub.  
![image](https://github.com/user-attachments/assets/04103aa9-5e41-4b78-93f8-268a5b19316c)  

There is a special tag that all images have which is called **latest**.  

## Getting a docker image
First, we search for the required image on the docker hub.  
Here, we will use **nginx**. 
Let us now select a specific version.  
![image](https://github.com/user-attachments/assets/fafd40a1-6082-447a-89a8-a00ff8b91017)


### docker pull <image_name>
We can use the below command to 
`docker pull nginx`  
or  
`docker pull <image_name>:<tag>`  which will mean:
`docker pull nginx:1.23`  
![image](https://github.com/user-attachments/assets/102257a3-60a3-4e45-824d-fa5b55ffe8f2)  

![image](https://github.com/user-attachments/assets/e71fd779-b4e0-458e-b6c1-a96c63b55456)  

This command will download the nginx image from the docker hub with the specified version.  
![image](https://github.com/user-attachments/assets/f52bb34b-b4f4-446f-a107-6074570b99de)  

Now, if we run the command `docker images`:  
![image](https://github.com/user-attachments/assets/194c9141-f5e4-461f-9245-93f40cb1937b)  

## Running a docker image
### `docker run <image_name> or docker run <image_name>:<tag>`  
The command for nginx becomes: `docker run nginx`  

Now, you can run the command: `docker ps` and see a list of containers currently running.  
![image](https://github.com/user-attachments/assets/60144f33-b784-412a-8372-5b637ef7a487)  

![image](https://github.com/user-attachments/assets/63eb833a-e87a-4da5-9c28-e22ee38296a7)  

When you run the docker container from the terminal, it will block the terminal. 
If you now press `ctrl+c` to stop the container.  
If you want to run a container in the background with it blocking the terminal use `-d` flag.  
`docker run -d ngnix`  

![image](https://github.com/user-attachments/assets/72f340be-85f2-4735-9cd5-559bf354e41a)  

Now, the logs for nginx will no longer be shown on the terminal. 
What if you want to see the logs for nginx which is running in the background without blocking the terminal? Use command:  
`docker logs <container_id>`  
![image](https://github.com/user-attachments/assets/6ecf6ad9-6d05-4518-bac9-98c149001044)  

## Flow so far..
![image](https://github.com/user-attachments/assets/fa83e672-d97a-4432-8cd6-7b82cced9383)  

We can skip the pull command:  
![image](https://github.com/user-attachments/assets/de50bab6-0d93-4dcf-babe-ee81d92514bc)  

You can use `docker run <image_name>` or `docker run <image_name>:<tag>`  
If docker does not find these images locally, it will pull them from the docker hub automatically.  

## Stopping a docker container  
Use command: `docker stop <container_id>`  
















































































 









































