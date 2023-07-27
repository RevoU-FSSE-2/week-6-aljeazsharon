[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/nj7iw4Wb)

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
WORKDIR instrustion sets the working directory for any instructions (RUN, CMD, COPY, ADD & ENTRYPOINT) in that follow Dockerfile.
COPY instruction copies new file or directory from and add them to file system of the container path.
RUN instruction will execute any commands in a new layer on top of the current image and commit the result.
EXPOSE instruction tell Docker that the container listens on the specified network ports at runtime.
CMD instruction specifies the command to run when a container is launched.
```

### Build Docker Image
1. write ```docker build -t week6``` (-t : nametag) on CMD or Terminal.
   
2. Run Container 
