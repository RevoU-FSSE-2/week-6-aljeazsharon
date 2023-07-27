![image](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/assets/25450018/62de02b3-970f-40fb-9e9e-d24e91a28a64)![image](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/assets/25450018/4d3c1287-8fc0-48c8-8e4a-3018f3993d4a)[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/nj7iw4Wb)

# Individual Assignment Week 06

## This week's assignment is about Docker with Node.Js with deliverables simple node.js project can be run inside a Docker container.

### Setting Up Docker on Your Machine
1. Download the [Docker for Windows](https://www.docker.com/products/docker-desktop/) Installation from the official Website.
   ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/01.png?raw=true)
   ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/02.png?raw=true)

 2. Install and configure the Docker Desktop.
    ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/03.png?raw=true)
    ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/04.png?raw=true)
    ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/05.png?raw=true)
    
 3. On Your Windows Machine, Docker Desktop will require a newer WSL kernel version.
    ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/07.png?raw=true)
    ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/08.png?raw=true)
   
 4. Create Docker Account (if you don't have one) or log in (If you have Docker Account)
    ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/10.png?raw=true)
    ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/11.png?raw=true)

 5. Verify the installation with CMD or Powershell by writing a command
    ```docker --version```
   ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/12.png?raw=true)

### Set up Node.Js Project

1. Download the simple node.js project from https://gist.github.com/berdoezt/e51718982926f0caa3fcd8ed45111430

   
2. Use Visual Studio Code to make a Dockerfile and package.json
   ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/13.png?raw=true)

```
FROM must be the first instruction in a Dockerfile. The FROM instruction initializes a new build stage and sets the base image for subsequent instructions.
The WORKDIR instruction sets the working directory for any instructions (RUN, CMD, COPY, ADD, and ENTRYPOINT) in the following Dockerfile.
The COPY instruction copies new files or directories and adds them to the file system of the container path.
The RUN instruction will execute any commands in a new layer on top of the current image and commit the result.
The EXPOSE instruction tells Docker that the container listens on the specified network ports at runtime.
The CMD instruction specifies the command to run when a container is launched.
```

### Build Docker Image
1. Write ```docker build -t week6``` (-t: nametag) on CMD or Terminal.
   ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/16.png?raw=true)
   
3. Run Container ```docker run -p 3002:3001 week6``` (-p: to publish or expose port)
   ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/17.png?raw=true)
   
4. Result
   ![alt text](https://github.com/RevoU-FSSE-2/week-6-aljeazsharon/blob/main/assets/18.png?raw=true)
