# Prodevans_linux
# Ansible Project - Automation Tasks

This repository contains a set of Ansible playbooks created as part of a project assessment.  
The tasks are designed to automate common administrative activities across CentOS and Ubuntu virtual machines.

## 📚 Playbooks Included

| Playbook | Description |
| `playbook_top5cpu.yml` | Find and display the top 5 CPU-consuming processes on the server. |
| `playbook_install_tomcat.yml` | Install Apache Tomcat server along with Java dependencies. |
| `playbook_fetch_time.yml` | Fetch and display the current system time using Ansible facts. |
| `playbook_create_user.yml` | Create a new user on the target systems. |
| `playbook_service_manage.yml` | Start and stop a specified service on Linux systems. |

## 🏗️ Setup Requirements

- Ansible installed on control node
- SSH access to both CentOS and Ubuntu VMs
- Sudo privileges on the target machines
- Python 3 installed on the target machines

## 📦 Inventory

An inventory file (`inventory.ini`) is included to define and manage the hosts.

Example structure:
```ini
[centos]
centos-vm ansible_host=192.168.1.10 ansible_user=youruser

[ubuntu]
ubuntu-vm ansible_host=192.168.1.11 ansible_user=youruser
