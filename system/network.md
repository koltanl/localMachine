# Network Configuration Context

## Interface Configuration
- **Primary Ethernet**: enp8s0 (UP, active)
  - IP: 192.168.123.114/24 (DHCP assigned)
  - Gateway: 192.168.123.1
  - Network: 192.168.123.0/24
- **Wireless**: wlp6s0 (DOWN, not in use)
- **Loopback**: lo (127.0.0.1/8)

## Network Setup
- **IP Assignment**: DHCP (dynamic)
- **Local IP Export**: $LOCAL_IP=$(ip route get 1 | awk '{print $7}') → 192.168.123.114
- **Routing**: Default route via 192.168.123.1 (metric 100)

## Network Services Status
Check system/services.md for active network-related services like:
- NetworkManager
- dhcpcd
- systemd-resolved
- Any custom firewall/iptables services

## HOMESERVER Network Context
For HOMESERVER debugging, this system likely:
- Connects to internal network (192.168.123.x)
- May have static routes to HOMESERVER services
- Could be running local services for development/testing
- May have VPN connections for remote access

## Common Network Tools Available
- ip (route, addr, link commands)
- systemctl (for network service management)
- netstat/ss (connection monitoring)
- ping/traceroute (connectivity testing)
- nmcli (NetworkManager CLI if installed)

## Firewall Status
- Check if nftables/iptables rules are active
- Look for custom firewall services in systemctl
- May have port forwarding rules for HOMESERVER services
