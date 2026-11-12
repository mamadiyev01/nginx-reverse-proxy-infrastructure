# Nginx Reverse Proxy Infrastructure

A hands-on infrastructure project demonstrating reverse proxy architecture using Nginx, MikroTik RouterOS, Ubuntu Server and Windows IIS.

## Project Overview

This project demonstrates how a centralized Nginx reverse proxy receives HTTP requests and forwards them to an internal backend web server.

The initial deployment uses one domain and one backend server. The architecture can be extended to support multiple domains and backend services.

## Network Architecture

```text
Windows Client
10.10.8.2
     |
     v
MikroTik Router
     |
     v
Ubuntu Server - Nginx
172.20.20.252
     |
     v
Windows Server - IIS
172.20.20.253
Technologies
- Ubuntu Server
- Nginx
- MikroTik RouterOS
- Windows Server
- IIS
- TCP/IP
- HTTP
- DNS
- Reverse Proxy
- Network Routing
Key Features
- Nginx reverse proxy deployment
- Backend web server integration
- HTTP request forwarding
- Network routing between subnets
- Domain-based virtual hosting (planned extension)
- Infrastructure documentation
Repository Structure
- docs/ - Architecture and technical documentation
- nginx/ - Nginx configuration examples
- mikrotik/ - Sanitized RouterOS examples
- backend/ - Backend server documentation
- monitoring/ - Health-check scripts
- screenshots/ - Project screenshots
Project Status
Initial single-domain reverse proxy deployment has been tested successfully.

HTTPS, multiple virtual hosts, monitoring and security improvements are planned.
Author
Ogabek Mamadiyev
