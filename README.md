# Firewalls-VPNs


# 🔒 Firewall Isolation Demo – Blocking Linux-to-Windows Communication

This repository documents a hands-on firewall configuration lab that simulates **host-level network isolation**. The goal is to block a Linux PC from initiating communication with a Windows PC using firewall rules, demonstrating access control and segmentation in a controlled environment.

## 🧪 Lab Objectives

- Configure firewall rules on Windows (using Windows Defender Firewall) and/or Linux (using UFW or iptables)
- Block inbound traffic from the Linux machine to the Windows host
- Test connectivity using ping, SSH, and other protocols
- Document rule behavior, test outcomes, and mitigation notes

## 🛠️ Environment Setup

- **Linux Host**: Ubuntu VM with UFW enabled
- **Windows Host**: Windows 10/11 VM with Defender Firewall
- **Network**: Shared virtual network or bridged adapter for direct IP communication

## 🚧 Rule Implementation (Example)

- On Windows: Create inbound rule to block traffic from Linux IP (e.g. `192.168.1.100`)
- On Linux: Optionally deny outbound traffic to Windows IP using `sudo ufw deny to 192.168.1.101`
- Test with `ping`, `telnet`, or `netcat` to confirm block

## 🛡️ Ethical Disclaimer

This lab is for **educational and professional development** only. All configurations are performed on non-production, consented systems. No unauthorized traffic manipulation or scanning is conducted.

