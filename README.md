# Infrastructure Automation with Vagrant, Ansible, and Docker
This project sets up a multi-node infrastructure environment using Vagrant and VirtualBox, automates server configurations using Ansible, and deploys a simple containerized app using Docker.

## Architecture
  - Control Node — manages all provisioning
  - 3 Managed Nodes — provisioned and configured automatically
  - Networking — Host-only network adapters
  - Application — Simple Dockerized app printing "Hello" and the server's IP

## Technologies Used
  - Vagrant
  - VirtualBox
  - Ansible
  - Docker
  - Ubuntu 18.04 (bento/ubuntu-18.04 box)

## How to Run
#### Clone this repository
``
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
``
#### Spin up the servers
``
vagrant up
``

#### SSH into the control node
``
vagrant ssh control
``
#### Run Ansible Playbook to configure nodes
``
ansible-playbook -i hosts ansible/playbook.yml
``

## Application Deployment
  - Each managed node will run a simple containerized app.

## Notes: 
  - Make sure VirtualBox and Vagrant are installed on your system.
  - Vagrant box used: bento/ubuntu-18.04
  - Host machine OS: (Specify your host OS here if you want, like Windows 10/11)

## License
This project is for learning and demonstration purposes.

## Quick Tip:
After you push it, make sure the repo has a clear name, like:

infrastructure-automation-lab

or

vagrant-ansible-docker-setup

Your commit message should be something simple but strong, like:

sql
Copy
Edit
Initial commit: Infrastructure Automation Lab using Vagrant, Ansible, and Docker
