# ansible_udemy
anisble_udemy assigment

# Solution
Below is my solution to the problem.

## Infrastructure
I chose Docker as I found it easiest to get started.

## Development Environment
I set up a local VM on Oracle Virtual Box as my Docker Engine.
After that installed below package to run the solution
 - Ansible
 - Python
 - Git

## Ansible Project
I decided to use tasks file for deploying contianer and create my own roles to configure those contianer with Application. I was not able to setup mailing due to docker env.​

Tasks: A role to deploy necessary Docker Contianers on the local VM.
Roles: create_docker_container: A role to validate Docker installtion status and configure Web and MySQL Contianers on the VM.
Roles: dependencies: A role to install and configure Flask application on multiple contianer

### Group Variables to have following properties:

- docker_network_name: network name for all the containers
- docker_container_details: ​ list of dictionary for docker contianer names and ports
- mysql_database_name: database name for mysql database
- mysql_user_name: database user name
- mysql_pass_name: password for database user

### There are few variable which i have declare in vars file of the roles.
