Role Name
=========

This role will harden and reconfigure your ssh server

Requirements
------------

The first step to configure SSH key authentication to your server is to generate an SSH key pair on your local computer.

To do this, we can use a special utility called ssh-keygen, which is included with the standard OpenSSH suite of tools. By default, this will create a 2048 bit RSA key pair, which is fine for most uses.

On your local computer, generate a SSH key pair by typing:

ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/home/username/.ssh/id_rsa):
The utility will prompt you to select a location for the keys that will be generated. By default, the keys will be stored in the ~/.ssh directory within your user's home directory. The private key will be called id_rsa and the associated public key will be called id_rsa.pub.



Role Variables
--------------

Set the ssh_port: Port 22 variable in vars/main.yml

Dependencies
------------

-

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD
