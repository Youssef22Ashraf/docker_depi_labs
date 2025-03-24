# docker_depi_labs - README

## Lab 1: Basic Docker Commands & Containers

### Problem 1: Hello World Container
- Run a basic `hello-world` container to verify Docker is working.
- Check container status.
- Restart a stopped container.
- Remove the container and its image.

### Problem 2: Running Interactive Containers
- Start an Ubuntu or CentOS container in interactive mode.
- Run `echo docker` inside the container.
- Create a file named `hello-docker`.
- Remove the container and note that temporary files are lost.

### Problem 3: Deploy MySQL Database
- Run a MySQL container with the name `app-database`.
- Use the `-e` flag to set `MYSQL_ROOT_PASSWORD`.
- Ensure the container runs in detached mode.

### Problem 4: Running Nginx with Static Files
- Start an Nginx container.
- Add static HTML files to the container.
- Verify that the files are accessible.
- Commit the changes to create a new image.

### Problem 5 (Bonus): Persistent Nginx with Volumes
- Attach a volume for static files.
- Remove the container and reattach the volume.
- Map port 80 to 9898 and access it in the browser.

---

## Lab 2: Dockerfiles & Custom Images

### Problem 1: Nginx with Volumes
- Run an Nginx container with two volumes (HTML files & config).
- Modify the HTML content.
- Restart the container using both **volume mount** and **bind mount**.
- Map port 80 to 8080 and verify accessibility.

### Problem 2: Custom Nginx Image
- Create a Dockerfile for an Nginx image with custom content.
- Modify the `nginx.conf` to listen on port **8080** instead of 80.
- Build and run the custom image.

### Problem 3: Containerizing a React App
- Create a ReactJS application.
- Write a Dockerfile to containerize it.
- Test the application inside a Docker container.
- **Bonus:** Optimize the image using multi-stage builds.

---

## Lab 3: Networking & Push to Docker Hub

### Problem 1: ReactJS & Docker Hub
- Build a React app container.
- Push it to **Docker Hub**.

### Problem 2: Ubuntu Sleep Container
- Write a Dockerfile for an **Ubuntu image** that sleeps by default for 5 seconds.
- Allow the sleep time to be overridden via **Docker command-line arguments**.
- Implement using **ENTRYPOINT and CMD**.

### Problem 3: Pushing Images to Docker Hub
- Tag and push the images from previous problems to Docker Hub.
- Ensure authentication and correct repository naming.

### Problem 4: Bridge Network with Nginx
- Create two Nginx containers on a custom **bridge network**.
- Use `curl` from one container to access the other’s content.
- Verify connectivity and test communication.

---

## How to Run the Labs
1. Clone the repository or create files manually.
2. Follow the steps in each lab.
3. Use `docker build`, `docker run`, and `docker network` commands as required.
4. Verify container output using `curl` or a web browser.

Let me know if you need modifications! 🚀
