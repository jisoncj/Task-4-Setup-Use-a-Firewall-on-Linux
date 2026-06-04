# Firewall Configuration Report
Tool: UFW (Uncomplicated Firewall)
System: Kali Linux
Date: June 2025

## What is a Firewall?
A firewall filters incoming and outgoing network traffic based
on rules. It acts as a barrier between your machine and the
outside world, allowing only authorized traffic through.

## Commands Used

### Enable firewall
sudo ufw enable

### Allow SSH
sudo ufw allow 22

### Block Telnet
sudo ufw deny 23

### Allow web traffic
sudo ufw allow 80
sudo ufw allow 443

### Check rules
sudo ufw status numbered.

## What I Learned
Firewalls work by matching traffic against a list of rules
from top to bottom. First match wins. Blocking unused ports
like Telnet (23) removes unnecessary attack surface. UFW makes
this simple with plain allow/deny commands instead of complex
iptables syntax.
