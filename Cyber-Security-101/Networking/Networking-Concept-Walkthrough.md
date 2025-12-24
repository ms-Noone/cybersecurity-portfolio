# 🖧 TryHackMe Walkthrough: Networking Concepts

## 📌 Room Overview
	• Difficulty: Easy
	• Estimated Time: ~60 minutes
	• Goal: Build foundational networking knowledge for cybersecurity
	
## 📝 Task 1: Introduction
This room is the first room in series of four room dedicated to introduce user to foundation of networking and most common networking protocol.

### Learning Objective:
	• ISO OSI network model
	• IP addresses, subnets, and routing
	• TCP, UDP, and port numbers
	• How to connect to an open TCP port from the command line

## 📝 Task 2: OSI Model
Open System Interconnection (OSI) model defines a framework for computer network communication. The OSI model is composed of 7 layers, each handling a specific function.

**Key Concepts:**
| Layer Number  | Layer Name | Main Function | Example of Protocol and Standards |
| ------------- | ------------- | ------------- | ------------- |
| Layer 7 | Application Layer | 	Providing services and interfaces to applications  | HTTP, FTP, DNS, POP3, SMTP, IMAP  |
| Layer 6  | Presentation Layer  | Data encoding, encryption, and compression  | Unicode, MIME, JPEG, PNG, MPEG  |
| Layer 5  | Session Layer  | Establishing, maintaining, and synchronising sessions  | NFS, RPC  |
| Layer 4  | Transport Layer | End-to-end communication and data segmentation  | UDP, TCP  |
| Layer 3  | Network Layer  | Logical addressing and routing between networks  | IP, ICMP, IPSec  |
| Layer 2  | Data Link Layer  | Reliable data transfer between adjacent nodes  | Ethernet (802.3), WiFi (802.11)  |
| Layer 1  | Physical Layer  | Physical data transmission media  | Electrical, optical, and wireless signals  |

👉 Mnemonic: _Please Do Not Trust Sale Person Advice_

### Flags/Answers:
	• End-to-end communication → Transport Layer (Layer 4)
	• Routing packets → Network Layer (Layer 3)
	• Encoding application data → Presentation Layer (Layer 6)
	• Same network segment transfer → Data Link Layer (Layer 2)

## 📝 Task 3: TCP/IP Model
TCP/IP Model is a Practical model developed by DoD for Internet use. One of the difference between OSI & TCP/IP model is in TCP/IP Model; the application layer encompassed of 3 OSI layers 5–7.

**Key Concepts:**  
- Layers: Physical, Data Link, Network, Transport, Application
	
### Flags/Answers:  
	• HTTP belongs to → Application Layer
	• Application layer covers → 3 OSI layers (5, 6, 7)

## 📝 Task 4: IP Addresses, Subnets & Routing
Every host on the networks need a unique identifier for other host to communicate with him. By using TCP/IP protocol suite, each device connected to the network will be assign their own IP. Below is the example of IP address:
![alt text](https://tryhackme-images.s3.amazonaws.com/user-uploads/5f04259cf9bf5b57aed2c476/room-content/5f04259cf9bf5b57aed2c476-1719849005781.png)


**Key Concepts:**  
- Router function is to forward data packet from resource to destination, this process is called Routing. Router function at layer 3.
- There is 2 Type of IP address:
  - Public IP : Assign by ISP for internet Access
  - Private IP:  Set by router for device communication within your home/ office network  
		Private IP ranges:  
				&emsp;- 10.0.0.0/8  
				&emsp;- 172.16.0.0/12  
				&emsp;- 192.168.0.0/16  
		
Command Examples:
Ifconfig or ipconfig : command to show IP address

Flags/Answers:  
• Not private → 49.69.147.197
• Invalid IP → 192.168.305.19


