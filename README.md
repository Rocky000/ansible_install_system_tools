# Ansible Install System Tools and Software
Recently, I was trying to automate the process of time conzuming and tring task that is installing softwares on a freshly installated Ubuntu Desktop.

I thought to make it a self-reliant Ansible for configuration management. That I can use to install any kinds of softwared as per needs and avoid the human error protion. 

This can be used for ubuntu servers too, you just need to comment out or remove the GUI based softwares.

# Values needed to be given before running the code
- On "hosts" file change the "<remote_IP>, <remote_user>, <remote_pass>,<local_user>,<local_pass>" with desired values
    Example: 192.168.0.100 ansible_connection=ssh ansible_user=abc ansible_password=abc
             127.0.0.1 ansible_user=abc ansible_password=abc ansible_become_password=abc

- on "./group_vars/all.yml" file change the values of following with desired version you want
# Ansible Playbook command
$ ansible-playbook -i ./hosts ./install_docker.yml

- Change the "hosts" value accroding to the hosts you want to run this ansible script "hosts: local" "hosts: install_soft"


