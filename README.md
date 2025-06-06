# Cyber Security Internship
## Task 8 - VPN Setup using ProtonVPN 

## Objective

To gain hands-on experience with VPNs and understand their role in protecting privacy and secure communication. This task was performed using **ProtonVPN Free Tier** and the built-in **VPN settings on Ubuntu**.

---

## Tools Used

- **ProtonVPN Free Tier**
---

## Steps Followed

### 1. Created a ProtonVPN Account
- Visited [ProtonVPN](https://protonvpn.com)
- Signed up for a free account

### 2. Downloaded VPN Configuration
- Navigated to the **Downloads** menu
- Scrolled down to download a **VPN configuration file** for Japan (`.ovpn`)
- You may select any country/server from the list provided
  ![image](https://github.com/user-attachments/assets/9431a875-a8d4-47a6-9e57-fd0f78b06872)

### 3. Retrieved OpenVPN Credentials
- Went to **Account > OpenVPN / IKEv2 section**
- Copied the **OpenVPN username and password**
- Saved these credentials in a text file for later use
![image](https://github.com/user-attachments/assets/02173467-fca9-425a-8fd9-d9f917d59ecc)

### 4. Imported VPN Configuration into Ubuntu
- Opened **Settings > Network > VPN**
- Clicked on the **'+' (Add VPN)** button
- Selected **'Import from file...'** and chose the downloaded `.ovpn` file
  ![image](https://github.com/user-attachments/assets/c06cb40a-6fd1-498d-8ae8-4d561626c81c)

### 5. Configured Identity Settings
- In the VPN details, selected the **Identity tab**
- Entered the **username and password** copied earlier
- Saved and connected to the VPN
  ![image](https://github.com/user-attachments/assets/a149f44d-0e9e-4157-b57a-fc94d838673f)

---

## Validation

### ✅ IP Address Before VPN
![image](https://github.com/user-attachments/assets/21e9ebd1-970a-4e83-b822-708e48c43180)

### ✅ IP Address After VPN
![image](https://github.com/user-attachments/assets/680e3a94-fc35-4a38-bd0d-b873f80cd9d7)

Verified using:
- https://nordvpn.com/what-is-my-ip/

---

### Encrypted Traffic Check
Successfully browsed Netflix while connected to VPN.
![image](https://github.com/user-attachments/assets/8b4e9436-f4cf-4a4c-a55e-6647e0784d4a)

- ***Connection is secure and certificate is valid***

---

### Network Speed Comparison
Used Internet Speed Test
without VPN:
![image](https://github.com/user-attachments/assets/51072bd5-d757-4b15-ba1d-d7f7760c7b24)
With VPN:
![image](https://github.com/user-attachments/assets/16a9380e-40ea-4665-9dc4-50d782b0af88)
fast but not good as without VPN

*VPN slightly reduced speed, but remained usable.*

---

## VPN Encryption and Privacy Features
## What is VPN Encryption?

A VPN (Virtual Private Network) encrypts internet traffic between your device and the VPN server, protecting data from:
- Hackers
- Government surveillance
- Internet Service Providers (ISPs)
- Public Wi-Fi threats

---

## Encryption Algorithms Used

VPNs employ robust encryption standards for both control and data channels:

| Channel         | Purpose                     | Algorithms Used                            |
|-----------------|-----------------------------|---------------------------------------------|
| Data Channel    | Encrypts transmitted data   | **AES-256-GCM**, AES-128, ChaCha20-Poly1305 |
| Control Channel | Secures key exchange & auth | **TLS 1.3**, RSA-4096, ECDHE                 |

- **AES-256-GCM**: Military-grade encryption used by most modern VPNs.
- **ChaCha20-Poly1305**: Lightweight and faster for mobile devices.
- **TLS 1.3**: Ensures secure handshake and session management.

---

## VPN Protocols

Protocols define the rules for secure data transmission:

| Protocol    | Features                                        | Common Use                        |
|-------------|-------------------------------------------------|-----------------------------------|
| OpenVPN     | Open-source, strong encryption, customizable    | Desktop clients (most secure)     |
| IKEv2/IPSec | Fast reconnect, mobile-friendly                 | Mobile devices                    |
| WireGuard   | Lightweight, high-speed, modern encryption      | Next-gen VPN services             |
| L2TP/IPSec  | Legacy support                                  | Outdated                          |
| PPTP        | Weak encryption, insecure                       | ❌ Avoid                          |

---

## Key Privacy Features

### Kill Switch
Automatically blocks internet access if VPN disconnects, preventing real IP exposure.

### DNS & IP Leak Protection
VPNs route DNS queries through encrypted tunnels, preventing DNS leaks. we can verify by accessing the links below:
- https://dnsleaktest.com
- https://ipleak.net

### Perfect Forward Secrecy (PFS)
Each session uses unique encryption keys. Even if one key is compromised, past sessions remain secure.

### No-Logs Policy
Trusted VPNs like ProtonVPN do not store:
- Browsing history
- Connection timestamps
- IP addresses

### Tor Over VPN 
Some providers allow routing VPN traffic through the **Tor** network for maximum anonymity.

---

## Summary Table

| Feature                 | Purpose                                        |
|--------------------------|------------------------------------------------|
| AES/TLS Encryption      | Protects data from interception                 |
| Kill Switch             | Prevents data leaks on disconnect               |
| No-Logs Policy          | Ensures privacy by not storing user activity    |
| Leak Protection         | Prevents DNS, IP, and WebRTC leaks              |
| Secure Protocols        | Uses trusted VPN protocols like OpenVPN         |
| PFS                     | Protects past sessions even if key is leaked    |

---

## References

- [ProtonVPN Features](https://protonvpn.com/)
- [OpenVPN Encryption Overview](https://openvpn.net/)
- [WireGuard Protocol](https://www.wireguard.com/)

## VPN Benefits

- Hides real IP and masks location
- Encrypts all network traffic
- Protects against Wi-Fi snooping
- Bypasses region-restricted content

---

## VPN Limitations

- Slightly reduces network speed
- May not work with some streaming services
- VPN provider can still log data (check privacy policy)
- Does not prevent phishing or malware attacks

---



## 👤 Done by

**Name**: Hemanth Kumar  
**Used Operating System**: Ubuntu Linux  
