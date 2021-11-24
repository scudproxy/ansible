# ansible
server and infrasatructure automation


files: description

hosts: machines you want to automate and connect to. <br />
hypervisor: hypervisor hosts\guests you want to manage

pb: ansible Playbooks

pb-service_account.yml: initial setup of service account and keys <br />
pb-ipv6_disable.yml: disables ipv6 on ubuntu only. 



[PB-SERVICE_ACCOUNT]
1. Make sure you have created a local service account on the controller node and is a sudoer
2. Initiate an initial SSH connection to the host you want to add to automationo
3. Make sure hosts file has accurate host names and your "local connection" defined

When ready to add a(some) host(s) run the following command as the destination computers root user

ansible-playbook /path/to/file/<playbook.yml> -i /p/t/f/<hosts> -l <[group]> -u <root> -kK



TBC
