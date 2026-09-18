# Mission Reflection

Docker containers boot up in seconds because they isolate processes while sharing the host operating system's kernel directly. In contrast, traditional Virtual Machines must emulate hardware, initialize a full guest OS, and load drivers, taking minutes to start.

Port mapping (`-p 8080:80`) is required because containers operate within isolated network namespaces. The Nginx service inside listens on internal port 80. Mapping host port 8080 to container port 80 routes incoming traffic from the host network directly into the isolated container.

When using `docker rm`, the container and its internal writable layer are permanently deleted. Any non-persistent data stored inside the container is lost unless attached to a Docker volume or bind mount.

Containerization transforms DevOps by standardizing execution environments. Developers bundle code and dependencies together into images, resolving "it works on my machine" issues and enabling seamless deployment across development and production environments.

Maintaining this GitHub portfolio tracks continuous hands-on learning in cloud infrastructure and cloud-native practices.
