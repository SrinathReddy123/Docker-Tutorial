15 Basic docker commands

1. Docker Version : Get the currently installed version of docker.

  docker --version
  
  <img width="240" alt="1 DockerVersion" src="https://user-images.githubusercontent.com/90196559/195874843-adbc84a5-f39c-48b0-a018-e87614d0f0e2.png">
  
2. Docker Login : Login to the docker hub repository.

   docker login
   
   <img width="850" alt="2 DockerLogin" src="https://user-images.githubusercontent.com/90196559/195874981-c43517ea-a900-4d7c-8bad-b43f98d0ddc8.png">

3.Docker Pull : Pull images from docker hub repository.  

    docker pull getting-started
    
    <img width="463" alt="3 DockerPull" src="https://user-images.githubusercontent.com/90196559/195875103-332bfc42-c94f-4f7b-86a4-67aaa4f62f9e.png">


4. Docker images : Lists all locally stored docker images.

    docker images
    
    <img width="348" alt="4 DockerImages" src="https://user-images.githubusercontent.com/90196559/195875198-43ea6bc7-8775-4719-8759-f74e0edd01d1.png">


5. Docker run : create container from the image. 

   docker run -d -p 80:80 docker/getting-started
   
   <img width="442" alt="5 DockerRun" src="https://user-images.githubusercontent.com/90196559/195875292-441489dd-9aad-47eb-b6d5-058b5920137b.png">


6. Docker ps : List all running container.

    docker ps 
    
    <img width="780" alt="6 Docker PS" src="https://user-images.githubusercontent.com/90196559/195875384-f6fbe0d2-8b39-43ec-8316-8b89fe06c25f.png">


7. Docker ps -a : List all containers, running and exited.

  docker ps -a
  
  <img width="725" alt="7 Docker PS -a" src="https://user-images.githubusercontent.com/90196559/195875444-905153ab-f1ee-4541-8c2e-014f467dfa75.png">


8. Docker rmi : Delete image.
 
  docker rmi hello-world
  
  <img width="515" alt="8 Docker Remove" src="https://user-images.githubusercontent.com/90196559/195875531-86938dc4-2a4a-46c6-a849-376e9c74847e.png">


9. Docker stop : Stops running container.

   docker stop getting-started  
   
   <img width="233" alt="9 Docker Stop" src="https://user-images.githubusercontent.com/90196559/195875616-c777860c-b6c5-47e2-83ed-f9fdf0b23a07.png">


10. Docker kill : Kills running container by stopping its execution  immediately. 
'docker stop' gives time to shutdown normally and 'docker kill'   shutdown immediately.   
   
     docker kill <container-id>
     
     <img width="800" alt="10 Docker Kill" src="https://user-images.githubusercontent.com/90196559/195875682-5e13a453-d47d-4e64-b7e8-96c272991c1b.png">


11. Docker rm : Removes container from local.

     docker rm <container-id>
    we cannot remove a running container, we should Stop the container before attempting removal or force remove     
 
    <img width="820" alt="11 Docker Rm" src="https://user-images.githubusercontent.com/90196559/195875795-db2cf1df-aba4-4e62-a157-f3347043faa2.png">

 12. Docker logs : Get logs of container.
  
   docker logs <container-id>
   
   <img width="529" alt="12 Docker Logs" src="https://user-images.githubusercontent.com/90196559/195875904-72a61760-170f-456d-abf3-2e26c191e911.png">


13. Docker build : Build docker image from specified docker file.

  docker build -t <image-name> .  
  
  <img width="639" alt="13 DockerBuild" src="https://user-images.githubusercontent.com/90196559/195875984-f6ce544d-f3af-4c4a-802e-8d8b66aaaab3.png">



14. Docker push : Push docker image from local to docker hub repository.

   docker push <username/image-name>:<tag-name>
   
   <img width="645" alt="14 DockerImageCreated" src="https://user-images.githubusercontent.com/90196559/195876054-212830ea-e5b6-4e17-b157-279bc4d25825.png">


15. Docker exec : Access running container.

    docker exec -it <container-name> bash
    
    <img width="661" alt="15 DockerPush" src="https://user-images.githubusercontent.com/90196559/195876146-6f7d1570-c592-4598-9edc-f891c5e819e4.png">
