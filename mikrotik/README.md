# MikroTik RouterOS - Network Routing

## Lab Network

### WAN
- Interface: ether1
- IP: 10.10.8.84/24
- Gateway: 10.10.8.1

### LAN
- Interface: ether2
- IP: 172.20.20.1/24

## Routing

Default route:
- Destination: 0.0.0.0/0
- Gateway: 10.10.8.1

Connected networks:
- 10.10.8.0/24
- 172.20.20.0/24

## NAT

Source NAT:
- Source network: 172.20.20.0/24
- Out interface: ether1
- Action: masquerade

## Reverse Proxy Traffic Flow

1. Client sends HTTP request.
2. Traffic reaches the network router.
3. Router forwards traffic to Nginx.
4. Nginx selects the backend using the hostname.
5. Nginx forwards the request to IIS.
6. IIS returns the response through Nginx.

## Security Notes

- Do not expose backend servers directly to the Internet.
- Allow only required ports.
- Use HTTPS for production.
- Do not publish passwords, private keys, tokens or full router backups.
