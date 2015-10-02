# Vagrant - Ansible 
Vagrant provisioning using ansible

# Vagrant
Vagrant is a tool for building complete development environments. With an easy-to-use workflow and focus on automation. https://www.vagrantup.com/

# Ansible
Ansible is a free software platform for configuring and managing computers. It combines multi-node software deployment, ad hoc task execution, and configuration management. http://docs.ansible.com/ansible/intro.html

# Installation
1. Install and configure VirtualBox, Vagrant and Ansible.
   1. VirtualBox https://www.virtualbox.org
   2. Vagrant http://docs.vagrantup.com/v2/getting-started
   3. Ansible http://docs.ansible.com/ansible/intro_installation.html
2. Open a shell prompt and cd into the folder containing the Vagrantfile
3. Run the following command to start the vagrant image 
   1. $ vagrant init precise32
   2. $ vagrant up
4. On the first vagrant up that creates the environment, provisioning is run. If the environment was already created and the up is just resuming a machine or booting it up, they won't run unless the --provision flag is explicitly provided.
5. You can also bring up your environment by using following command
   1. $ vagrant provision

# About Author
Rolind Roy https://in.linkedin.com/in/rolindroy
Reach out if you want to talk - rolind.roy@gmail.com 
