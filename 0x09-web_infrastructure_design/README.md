# Web Infrastructure Project README

This project aims to design a scalable and fault-tolerant web infrastructure using a split-component architecture with a load balancer and dedicated servers for each component.

## Architecture Overview

The infrastructure consists of the following components:

- **Load Balancer (HAproxy)**: Responsible for distributing incoming traffic across multiple instances of web and application servers.
- **Web Server**: Serves static content and handles HTTP requests from clients.
- **Application Server**: Executes the application codebase and generates dynamic content.
- **Database Server (MySQL)**: Stores and manages application data.

## Installation and Setup

1. **Load Balancer (HAproxy)**:
   - Install HAproxy on a dedicated server.
   - Configure HAproxy as a cluster with another HAproxy instance for high availability.

2. **Web Server**:
   - Install and configure a web server (e.g., Nginx or Apache) on a dedicated server.
   - Serve static content and proxy dynamic requests to the application server.

3. **Application Server**:
   - Install and configure an application server (e.g., Node.js, Django, or Flask) on a dedicated server.
   - Execute the application codebase and handle dynamic content generation.

4. **Database Server (MySQL)**:
   - Install and configure MySQL on a dedicated server.
   - Set up databases and manage application data.

## Usage

- Start by configuring each server according to its role (load balancer, web server, application server, database server).
- Ensure proper communication between components by configuring network settings and firewall rules.
- Monitor server performance, traffic, and resource utilization using appropriate monitoring tools.

## Contributing

Contributions are welcome! If you have suggestions, feature requests, or bug reports, please open an issue or submit a pull request.

