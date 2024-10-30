# PT START. INT-4 DevOps. Ansible

This repository contains an Ansible playbook for the basic configuration of a Debian 11 server and the installation and setup of PostgreSQL 16.

## Steps to Run

1. Add Ansible User:
   - Ensure that the user ansible exists on the target machine (Debian 11). This user should have the necessary permissions for configuration.

2. Inventory Setup:
   - Create an inventory file (for example, hosts.ini) with the following content:
     
     myHost ansible_host=<ip addr> ansible_user=ansible ansible_password=ansible
     
   - Replace <ip addr> with the actual IP address of your target machine.

3. Run the Playbook:
   - Execute the following command to run the playbook:
     
     ansible-playbook configurate_debian11_postgresql_playbook.yml -k
     
   - The -k flag will prompt you to enter the password for the ansible user on the target machine.

## Conclusion

After running the playbook, your Debian 11 server will be configured, and PostgreSQL 16 will be set up and ready for use.
