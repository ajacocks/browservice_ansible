# browservice_ansible
This is an Ansible deployer for the browservice vintage web proxy service. See https://github.com/ttalvitie/browservice for the serrvice that it deploys.

By default, this playbook needs a group created, in your Ansible inventory, called `browservice`. It will attempt to install the browservice software on all hosts in that group.

Right now, only Fedora hosts are supported. Please let me know if you would like support for other Linux distributions.

Variables affecting installation are in group_vars/browservice.yml

You can install browservice on a host by:

1) adding that host to ansible's [browservice] group
2) ansible-playbook main.yml --extra-vars '{"local_service":true}'

You can install browservice, in a container, on a host by:

1) adding that host to ansible's [browservice] group
2) ansible-playbook main.yml --extra-vars '{"container_service":true}'

Please let me know if you find any issues, or have suggestions.

- Alexander Jacocks
alexander@redhat.com
