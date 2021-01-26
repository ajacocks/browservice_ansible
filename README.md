# browservice_ansible
This is an Ansible deployer for the browservice vintage web proxy service. See https://github.com/ttalvitie/browservice for the serrvice that it deploys.

By default, this playbook needs a group created, in your Ansible inventory, called `browservice`. It will attempt to install the browservice software on all hosts in that group.

Right now, only RHEL/CentOS and Fedora hosts are supported. Please let me know if you would like support for other Linux distributions.

- Alexander Jacocks
alexander@redhat.com
