# Ansible-POC
This Repository is configured to trigger a job in Jenkins whenever 'push' command is executed.
So whenever there is a push to this repository there will be a job triggered in the Jenkins server that is configured with this repository and that job will run the ansible playbook against the hosts machines which are mentioned in the 'hosts' files.

### The ansible.cfg file
In this file we will specify all the configuration required by Ansible for configuring the remote machine like with which user should be used to connect to remote machines and the which public key to be used to connect to the remote machine and alot of other configurations can be done in this file.

### The hosts file
In the hosts file we can specify the hosts that we want to configure. We can group a set of machines that should be configured differently.

### The default-playbook.yml file 
This is the playbook that will be executed on the remote machines. Here we can specify all the commands that should be executed. 
