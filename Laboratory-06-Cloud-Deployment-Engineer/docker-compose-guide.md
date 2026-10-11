# Docker Compose Guide

## What does the services: block do?
The `services:` block defines the individual containers (or services) that make up your multi-container application stack. Under this block, you declare each service (such as `database` and `app`), specify their container images, define port mappings, set environment variables, and configure networking rules so Docker knows how to build and launch them together.

## How did the Nextcloud app container find the database container?
The Nextcloud app container located the database container using the `MYSQL_HOST=database` environment variable. Docker Compose automatically creates a default internal bridge network for all services defined in the YAML file and handles internal DNS resolution. Because our database service is named `database`, other containers on the same network can reference it directly by that hostname.

## Difference between `docker run` and `docker-compose up -d`
* **`docker run`**: Executes a manual command to deploy a *single* container at a time. If you have a multi-tier application, you must manually create networks, link containers, specify individual storage flags, and run multiple commands sequentially, making it prone to human error.
* **`docker-compose up -d`**: Uses Infrastructure as Code (IaC) principles via a `docker-compose.yml` blueprint. It reads the entire multi-container architecture specification and deploys, links, and runs the entire stack simultaneously in the background (`-d`) with a single command.
