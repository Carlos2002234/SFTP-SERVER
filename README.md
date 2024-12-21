# Project Name: Secure SFTP Server Setup

## Overview
This project provides a secure and customizable SFTP server setup using best practices for file transfer. The server is configured to allow SSH key-based authentication, ensuring passwordless logins. It incorporates security features such as user isolation with a chroot environment, automatic IP blocking using fail2ban, and firewall configuration to limit access to only necessary ports and trusted IPs. This setup ensures secure file transfers and protects against unauthorized access.

**Example:**
This project provides a step-by-step guide for setting up a secure FTP server with advanced security measures.

---

## Prerequisites
Before you begin, ensure you have met the following requirements:

- Ubuntu or Debian-based OS
- OpenSSH Server installed
- Fail2ban (optional but recommended for enhanced security)
- UFW firewall (optional for additional security)
- Basic knowledge of server administration and SSH

---

## Steps to Set Up

### Step 1: Install and Update the System
1. Update the system and install necessary packages.
   
   ```bash
   sudo apt update && sudo apt upgrade -y
   sudo apt install openssh-server -y
