# 🛠️ NMAP – Command Cheat Sheet  
This cheat sheet was created to capture useful commands for quick future reference

| Feature | Command  | Description |
| ------------- | ------------- | ------------- |
| Host Discovery | `nmap -sn IP` | Discover live host without probing services |
| Host Discovery | `nmap -sL IP` | List live host without scanning |
| Port Scanning | `nmap -sT IP` | TCP Connect scan by complete full handshake |
| Port Scanning | `nmap -sS IP` | TCP Syn scan |
| Port Scanning | `nmap -sU IP` | UDP scan |
| Port Scanning | `nmap -p- IP` | Scans all ports |
| Version Detection | `nmap -sV IP` | Service and Version detection |
| OS Fingerprinting | `nmap -O IP` | OS fingerprinting |
| Version & OS detction | `nmap -A IP` | OS detection, version detection, and other additions | 
| Verbosity | `nmap IP -v` | Real-time Scan Progress |

