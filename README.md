# muni-pa160-ansible
Example of ansible-pull for the course PA160 at Masaryk University

Create a Debian 10 virtual machine in cloud with public IP address.

Start managing it with Ansible pull by issuing the following commands as root on it:
```bash
apt update
apt install ansible git
ansible-pull -U https://github.com/martin-kuba/muni-pa160-ansible.git
```

The playbook [local.yml](local.yml) is refreshed and executed every 5 minutes then.

It installs a [Chat Service](https://github.com/martin-kuba/muni-pa160-chat-service)
to run on port 8080.

