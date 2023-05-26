# Ansible

## what ansible stand for?

Ansible is an open-source configuration management and task automation platform. It enables large-scale IT systems to be deployed, configured and managed simply and reproducibly.

## Things you need to know about Ansible

1. Client-server architecture: Ansible follows a client-server architecture with a controller and managed nodes.

2. The inventory is a file that lists the remote machines on which you wish to perform actions.

3. Playbooks: Playbooks are YAML files that describe the tasks to be performed on managed nodes.

4. Modules: Ansible uses modules to perform specific actions on managed nodes.

5. Tasks: Tasks are actions to be performed on managed nodes and are associated with modules.

6. Ad-hoc commands: Ansible lets you execute ad-hoc commands without creating a playbook.

### Install Ansible

Before using Ansible, our first reflex is to install it on our linux. <br>

first, we need to update our linux and our package. Use the following commands:

```
` sudo apt update` <br>
`sudo apt upgrade ` <br>
```
To do this, simply type the following command:

```
`sudo apt install ansible`
```