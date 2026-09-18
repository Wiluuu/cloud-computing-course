# Docker Deployment & Command Explanations

- `docker version`: Displays version details for both Docker client and server engines.
- `docker info`: Displays system-wide information regarding total containers, images, and configuration settings.
- `docker pull nginx`: Downloads the official Nginx container image from Docker Hub to the local host.
- `docker run -d -p 8080:80 --name my-nginx nginx`: Runs the Nginx container in detached mode (-d), names it my-nginx, and maps host port 8080 to container port 80.
- `curl http://localhost:8080`: Sends an HTTP request to verify that the Nginx web server is active and serving web pages.
- `docker ps`: Lists all currently running containers.
- `docker stop my-nginx`: Gracefully stops the running Nginx container.
- `docker ps -a`: Lists all containers on the host, including stopped ones.
- `docker rm my-nginx`: Permanently deletes the stopped container from the system.
