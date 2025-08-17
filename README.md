# docker
This repository has docker related documents and images created for learning

## Learning Progress
Following the [Docker Roadmap](https://roadmap.sh/docker) for structured learning.

## Daily Learning Tracker

### 16-08-2025
**Topic:** *Basic Docker Images and Container*   
**Commands/Code:**  
```bash
docker images
docker ps
docker build -t node-app .
docker run -p 3000:3000 node-app:latest

# Pull image from docker registry
docker pull <image-name>:tag

# Run a container in interactive mode
docker run -it node:latest
```
**Notes:** 
<details>

- Create a simple Dockerfile to intall node and run the sample node js application
- Added .dockerignore to ignore unnecessary files.
- Created an image node-app:latest with this file.
- Used docker run to spin up a container which is accessible on port 3000
- Pulled a image directly from docker hub and ran an interactive container with it.
- Docker uses layer based architecture to build images. Due to which it will execute the instructions which is changed along with all the instructions after that.


</details>

---
### 17-08-2025
**Topic:** *Basic operations on images and containers*
**Commands/Code:**  
```bash
# Execute a container in detach mode
docker run -p port:port -d <image-name>:tag
# Start an existing container
docker start <container_id>
# Attach a running container
docker attach <container_id>
# Start a container in attach mode
docker start -a <container_id>
# View log of a container
docker logs <container_id>
# Follow the future logs
docker logs -f <container_id>
# Run a container in interactive mode
docker run -it <image_id>
# Start an existing container in interactive modoe
docker start -i <container_id>
# Delete image
docker rmi <image_id1> <image_id2>
# Delete container
docker rm <container_id1> <container_id2>
# Remove unused untagged images
docker image prune
# Remove container when exit
docker run -p port:port -d --rm <image_id>
# Details of an image
docker image inspect <image_id>
# Copy file to or from running container
docker cp <local_path> <container_id>:<path_in_container>
docker cp <container_id>:<path_in_container> <local_path>
```
**Notes:** 
<details>

- Starting a container with *docker start* command, will start it in detached mode.
- All the commands accept image_id or image_name.
- All the commands accept both container_id and container_name.
- If a container needs user input at runtime, it can be executed in interactive mode.
- First container using an image has to be removed then only image can be removed.


</details>

---

### Template for New Entries
**Topic:**  
**Commands/Code:**  
```bash
# Add commands here
```
**Notes:** 
<details>

- What I learned
- Challenges faced
- Things to remember

</details>


