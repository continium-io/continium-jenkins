Continium Jenkins installation.
=========

This role installs Jenkins and Default Jre on a newly created server.
It is not recommended to run on the product server or a server under development.


Requirements
------------

No spesific requirements. 

Ansible installed linux server is required to run this role. In addition, there must be the necessary elements(root password, ssh key) for the ssh connection to the server where the role will run.

You can use the following commands to install Ansible (Only Debian systems):

    $ sudo apt-get install software-properties-common 
    $ sudo apt-add-repository ppa:ansible/ansible 
    $ sudo apt-get update 
    $ sudo apt-get install ansible

For more: https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html


Role Variables
--------------

This role have 4 variables in defaults. They are Jenkins repository and repo's key. No needed change. 

Dependencies
------------

It has no dependencies.


Example Playbook
----------------

How to write playbook?

  jenkins.yml:

    - hosts: Jenkins-Server
      roles:
         - continium.ansible-jenkins.install


How to run playbook?

    ansible-playbook jenkins.yml    


License
-------

BSD

Author Information
------------------

Emre Aydınsoy. 

DevOps Engineer