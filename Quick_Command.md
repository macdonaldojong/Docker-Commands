# Learn Docker & commands

## Before Containers?

![image](https://user-images.githubusercontent.com/58276505/172675280-cd43db25-4b2c-43ac-84b1-74b9806e39d8.png)

## But after the presence of containers?

![image](https://user-images.githubusercontent.com/58276505/172675507-7a85ad98-95c8-4664-b09f-d7a320ea6fc6.png)

All what is needed is to install docker and 1 command to have it running on our local machines

* For example to run postgress db locally -> to docker website -> type postgress & select from original image, the version you need & run command to install:

![image](https://user-images.githubusercontent.com/58276505/172677240-40db547a-4b0b-463f-86ce-97462ae5bbdf.png)

### command to just install a container:
-  => docker pull image_name
-  then run it with
-  => docker run command

### command to Install & run a conatainer
```
*  => docker run postgress:9.6                   (where: postgress:10.10 => image_name: version number )                                  
```
![image](https://user-images.githubusercontent.com/58276505/172681904-a800e5d7-140b-4aa3-9f0e-52c29c56cc9e.png)

### command to verify conatainers installed
```
- => docker ps                                     (command to verify conatainers installed)                                  
```

![image](https://user-images.githubusercontent.com/58276505/172680904-2bd3113b-53b3-404d-8e2e-07032ce6fa75.png)

## Difference between image & container in docker?
![image](https://user-images.githubusercontent.com/58276505/172678459-f6f3844b-3991-446b-97f1-4ab3ae4fdac4.png)

## Difference between Docker & Virtual Machine?
![image](https://user-images.githubusercontent.com/58276505/172685961-dc406a98-be4b-4862-9834-2cd2b564be79.png)
- Docker container uses the OS of host machine meanwhile VM are install with their own os
- Speed: Docker container start & run faster compared to VM
- Size: Docker container images are smaller ()
- Compactibity: VM of any OS can run on any OS host but docker doesn't run well on all windows version kernel below 10 (except install docker toolbox to the kernel)

![image](https://user-images.githubusercontent.com/58276505/172686170-84ea5f92-fb3f-4db3-965e-c81369122f74.png)

## Install Docker: Mac , Windows 10-> (less than 10, install docker toolbox), linx
* Create a repository and setup the download instructions for download, installer & dependencies for various OS and then use cmd [sudo add-apt-repository]
* For Linux & Mac: Open official documentation community & enterprise version, download installer corrsponding to your OS.
* For Windows: You must enable hyper-V & then run installer (All windows version below 10, can't run docker except Docker toolbox must be installed)

## Useful command for docker:
*  => docker pull 'image_name'
*  => docker run --name                      (docker run creates a new container; --name= 'image_name:version')
*  => docker run -d -p --name                (-d = detachable, -p= specify port, --name= specify image &/version eg {docker run -d -p'6000:6794})
*  => docker ps ........................     (To show installed containers)
*  => docker run -d 'image_name:latest' ..........  (runs docker container in a detached mode (allowing you to use terminal) + the container id) 
*  => docker stop / start 'id_container' ... (To stop & restart a running container, use its container_id; get container_id from history by running {docker ps-a})
*  => docker ps -a ......................... (To get history of all container both running & non-running )
*  => ctrl+c  ...............................(To terminate )
* => docker exec -it 'ID' /bin/bash
* => Exit
* => docker pos
* => 
![image](https://user-images.githubusercontent.com/58276505/172697647-f48a9175-c10c-415d-9327-220433edcf25.png)

## How to use containers:
![image](https://user-images.githubusercontent.com/58276505/172699104-c4cd3709-c3bb-407c-93b2-dfec933f8b64.png)

* For 2 or more containers running on same port will signal error:
* Solution is to Bin then to a specific Port eg 6000 [docker run -d -p'6000:6794']

![image](https://user-images.githubusercontent.com/58276505/172701928-fd121a45-23cf-476e-99f4-ef68a564d9db.png)

### To change docker ports

*  => docker run -d -p'6000:6794 ......... In above example (host_port:container_port) where, host_port = 6000 ,,,,6001,,,,,6002 & container_port= 6794

![image](https://user-images.githubusercontent.com/58276505/172704010-545ae5fb-41ff-49fa-b497-3c81a69ad761.png)

## Trouble shouting a container
* => docker ps            (se container details but no logs)
* => docker logs 'ID'     (put specific container ID to see it's logs)
* => docker logs 'container_name'     (put specific container container_name to see it's logs)

![image](https://user-images.githubusercontent.com/58276505/172763784-b14acead-f728-412c-af0f-692f6f5478d0.png)
* docker exec -it 'ID' /bin/bash     (get the terminal of a container to check anything as user/root) (Always specify ID=container id)
* Exit  (To exit the container)

![image](https://user-images.githubusercontent.com/58276505/172764636-ecac5493-4a8d-4e46-9b1e-87b4a93ab6b7.png)

## USE of Docker

![image](https://user-images.githubusercontent.com/58276505/172766502-0e669156-53f2-4e25-9864-b4d4052272ba.png)

![image](https://user-images.githubusercontent.com/58276505/172767215-05c9d572-bb09-4e7b-a964-db9c45dd515d.png)

![image](https://user-images.githubusercontent.com/58276505/172767708-a50bfd59-1cc7-4cbc-8739-4b5ae1141282.png)


## Check application code here => https://www.youtube.com/watch?v=3c-iBn73dDE&t=1156s
