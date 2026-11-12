# Network Architecture

## Components

| Component | Role | IP Address |
|---|---|---|
| Windows Client | HTTP Client | 10.10.8.2 |
| MikroTik Router | Gateway | 10.10.8.84 |
| Ubuntu Server | Nginx Reverse Proxy | 172.20.20.252 |
| Windows Server | IIS Backend | 172.20.20.253 |

## HTTP Request Flow

1. Client requests ogabek.uz.
2. DNS resolves the domain to the Nginx server.
3. Client connects to Nginx.
4. Nginx receives the HTTP request.
5. Nginx forwards the request to Windows IIS.
6. IIS returns the response to Nginx.
7. Nginx sends the response to the client.

## Technologies

- Nginx Reverse Proxy
- MikroTik RouterOS
- Ubuntu Server
- Windows IIS
- TCP/IP
- HTTP
- DNS

## Security Note

This is a private laboratory environment.
IP addresses are provided for documentation purposes.
