# Laboratory 04: The Cloud-Native Engineer

## Mission Overview
Explored containerization fundamentals by transitioning from VMs to Docker containers using KillerCoda. Successfully pulled, deployed, verified, and managed an Nginx web server container.

## Objectives
- Differentiate between VMs and Containers.
- Access Docker environment on KillerCoda.
- Execute basic Docker CLI commands.
- Manage container lifecycles.
- Document procedures using Markdown.

## Docker Commands Executed
- `docker version`
- `docker info`
- `docker pull nginx`
- `docker run -d -p 8080:80 --name my-nginx nginx`
- `curl http://localhost:8080`
- `docker ps`
- `docker stop my-nginx`
- `docker ps -a`
- `docker rm my-nginx`

## Skills Learned
- Container process isolation and port forwarding mechanics.
- Managing ephemeral container states.

## Challenges Encountered
- Verifying network traffic routing via local port mapping before testing curl output.
