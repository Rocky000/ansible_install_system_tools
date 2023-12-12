# Ansible Install System Tools and Software
Recently, I was trying to automate the process of time conzuming and tring task that is installing softwares on a freshly installated Ubuntu Desktop.

I thought to make it a self-reliant Ansible for configuration management. That I can use to install any kinds of softwared as per needs and avoid the human error protion. 

This can be used for ubuntu servers too, you just need to comment out or remove the GUI based softwares.

# Values needed to be given before running the code
- On "hosts" file change the "<Destination_Host_IP>, <User_Name>, <User_Password>" with desired values
    Example: 192.168.0.100 ansible_connection=ssh ansible_user=abc ansible_password=abc

- on "./group_vars/all.yml" file change the values of following with desired version you want
    python3_version: python3.10
    node_version: v16.14.0 
# Ansible Playbook command
$ ansible-playbook -i ansible_install_system_tools/hosts ansible_install_system_tools/install_docker.yml


