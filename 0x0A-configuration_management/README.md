# 0x0A. Configuration management

The project is about working with Puppet as a configuration management tool, practicing writing Puppet manifest files to create a file, installing a package, and executing a command.

# TASKS:

## Task0:

### 0. Create a file

Using Puppet, create a file in /tmp.

Requirements:

	- File path is /tmp/school
	- File permission is 0744
	- File owner is www-data
	- File group is www-data
	- File contains I love Puppet

## Task1:

### 1. Install a package

Using Puppet, install flask from pip3.

Requirements:

	- Install flask
	- Version must be 2.1.0

## Task2:

### 2. Execute a command

Using Puppet, create a manifest that kills a process named killmenow.

Requirements:

	- Must use the exec Puppet resource
	- Must use pkill
