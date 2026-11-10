# module-02-linux-networking-cloud-infrastructure
Module 02: Linux, Networking & Cloud Infrastructure

Overview

This repository contains my practical work and learning notes for Module 02 of the Cloud & DevOps internship at Codomax.

The module focuses on Linux fundamentals, networking concepts, secure remote access and deploying a service in a Linux environment.

Learning objectives

* Navigate the Linux command line.
* Manage files, directories and permissions.
* Understand Linux users and groups.
* Monitor and manage processes.
* Manage Linux services using systemd and systemctl.
* Understand IP addressing and DNS.
* Identify network ports and protocols.
* Understand firewalls and AWS Security Groups.
* Configure SSH key-based authentication.
* Deploy and test a web service.

Environment

Component	Configuration
Host operating system	Windows 11
Linux environment	Ubuntu on WSL2
Service deployed	Nginx
Web protocol	HTTP
HTTP port	80
SSH port	22
SSH authentication	Public/private key authentication

Environment note: The practical exercises were performed using Ubuntu on Windows Subsystem for Linux 2 (WSL2). WSL2 provides a Linux environment using a lightweight virtual machine. It is not the same as independently provisioning and managing a standalone virtual machine using a hypervisor or cloud platform. This distinction is recorded transparently.

Practical work completed

1. Linux fundamentals

* Navigated the Linux filesystem.
* Created, copied, moved and removed files and directories.
* Inspected file permissions.
* Applied permissions using chmod.
* Created a Linux user and group.
* Configured shared directory ownership and permissions.
* Worked with Linux processes.
* Managed services using systemctl.

2. Networking fundamentals

* Inspected network interfaces and IPv4 addresses.
* Tested network connectivity using ping.
* Tested DNS resolution using getent hosts.
* Inspected DNS resolver configuration.
* Identified listening ports using ss.
* Tested HTTP connectivity using curl.

3. SSH configuration

* Generated an Ed25519 SSH key pair on Windows.
* Added the public key to Ubuntu’s authorized_keys file.
* Configured SSH directory and file permissions.
* Verified that public-key authentication was enabled.
* Connected from Windows PowerShell to Ubuntu using SSH key authentication.

The private key remains on the Windows host. Only the public key was added to Ubuntu.

4. Service deployment

* Installed Nginx on Ubuntu.
* Started and enabled the Nginx service.
* Verified that Nginx was listening on port 80.
* Accessed the Nginx welcome page through http://localhost in the Windows browser.

Firewall and cloud security

Firewall concepts and AWS Security Groups are included in the learning notes.

UFW and nftables were not available in the Ubuntu environment during the practical checks. No firewall configuration was changed or claimed as completed.

AWS Security Groups are virtual firewalls associated with AWS resources such as EC2 instances. Their inbound and outbound rules control permitted traffic.

No AWS infrastructure was provisioned for this practical exercise.

Repository structure

* linux/ – Linux commands, users, permissions and process management.
* networking/ – IP addressing, DNS, ports, protocols and firewalls.
* server-deployment/ – SSH configuration, Nginx deployment and connectivity testing.
* screenshots/ – Practical evidence.
* scripts/ – Supporting scripts, if applicable.

Key learning outcome

This module provided practical exposure to Linux administration, network troubleshooting, SSH security and web server deployment. It also strengthened my understanding of how Linux services communicate over network ports and how secure access is configured.

Technologies and tools

* Ubuntu
* WSL2
* Linux CLI
* OpenSSH
* Nginx
* HTTP
* DNS
* TCP/IP
* Windows PowerShell
* AWS Security Groups (conceptual learning)