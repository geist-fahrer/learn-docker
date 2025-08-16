# docker
This repository has docker related documents and images created for learning

## Learning Progress
Following the [Docker Roadmap](https://roadmap.sh/docker) for structured learning.

## Daily Learning Tracker

### 2025-08-16
**Topic:*Basic Docker Images and Container*   
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

### Template for New Entries
**Topic:**  
**Commands/Code:**  
```bash
# Add commands here
```
**Notes:** 
<details>
<summary>Learning Summary</summary>

- What I learned
- Challenges faced
- Things to remember

</details>


