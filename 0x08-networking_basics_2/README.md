# 0x08. Networking basics #1

# Resources

## Read or watch:

[What is localhost](https://en.wikipedia.org/wiki/Localhost)<br>
[What is 0.0.0.0](https://en.wikipedia.org/wiki/0.0.0.0)<br>
[What is the hosts file](https://www.makeuseof.com/tag/modify-manage-hosts-file-linux/)<br>
[Netcat examples](https://intranet.alxswe.com/rltoken/OR0lOEwAw9I1Rj4aGp1Ljg)<br>

### man or help:

	- ifconfig
	- telnet
	- NC
	- cut

# Learning Objectives

At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

## General

	- What is localhost/127.0.0.1
	- What is 0.0.0.0
	- What is /etc/hosts
	- How to display your machine’s active network interfaces


# Requirements

## General

	- Allowed editors: vi, vim, emacs
	- All your files will be interpreted on Ubuntu 20.04 LTS
	- All your files should end with a new line
	- A README.md file, at the root of the folder of the project, is mandatory
	- All your Bash script files must be executable
	- Your Bash script must pass Shellcheck (version 0.7.0 via apt-get) without any errors
	- The first line of all your Bash scripts should be exactly #!/usr/bin/env bash
	- The second line of all your Bash scripts should be a comment explaining what is the script doing

# TASK 0

### 0. Change your home IP

Write a Bash script that configures an Ubuntu server with the below requirements.

Requirements:

	- localhost resolves to 127.0.0.2
	- facebook.com resolves to 8.8.8.8.
	- The checker is running on Docker, so make sure to read [this](http://blog.jonathanargentiero.com/docker-sed-cannot-rename-etcsedl8ysxl-device-or-resource-busy/)<br>

# TASK 1

### 1. Show attached IPs

Write a Bash script that displays all active IPv4 IPs on the machine it’s executed on.

# TASK 2

### 2. Port listening on localhost

Write a Bash script that listens on port 98 on localhost.
