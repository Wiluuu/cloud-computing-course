# Mission Reflection

Object storage is better suited for storing millions of photos than a traditional block storage drive because it is built to scale. Block storage behaves like a single disk with fixed capacity, so growing it means resizing volumes or adding disks and managing them manually. Object storage keeps each file as an object with a unique ID and metadata in a flat structure, and it can grow almost without limit. It is also accessed over HTTP, which makes it easy for a web application to upload and retrieve images from anywhere.

Docker made deploying MinIO much easier because I did not have to install or configure anything manually. A single `docker run` command downloaded the image, set the admin credentials through environment variables, mapped the ports, and started the server in seconds. Since the container is self-contained, the same command should work on any machine with Docker. **[Add one thing that surprised you or went wrong, e.g., using the Chainguard image.]**

A bucket is a top-level container in cloud storage that holds objects (files). It is similar to a folder, but it is a flat namespace where each object is identified by a unique key, and access rules are usually applied at the bucket level. In this lab, I created a bucket named `client-photos` and uploaded a test file into it.

Large enterprises protect object storage data from server failures through redundancy. Data is replicated, or split using erasure coding, across multiple drives, servers, and even data centers or regions. If one physical machine crashes, the other copies can rebuild and serve the data. This is how services like Amazon S3 achieve very high durability. **[Add a source you looked up.]**

My confidence in the Linux command line is growing. Commands like `docker run`, `docker ps`, and `docker logs` now make more sense, and I understand what flags like `-d`, `-p`, and `-e` do instead of just copying them. **[Be honest about what still feels difficult.]**
