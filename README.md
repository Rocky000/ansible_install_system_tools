# Ansible Install System Tools and Software
Recently, I was trying to automate the process of time conzuming and tring task that is installing softwares on a freshly installated Ubuntu Desktop.

I thought to make it a self-reliant Ansible for configuration management. That I can use to install any kinds of softwared as per needs and avoid the human error protion. 

This can be used for ubuntu servers too, you just need to comment out or remove the GUI based softwares.

# Ansible Playbook command
$ ansible-playbook -i ansible_install_system_tools/hosts ansible_install_system_tools/install_docker.yml
