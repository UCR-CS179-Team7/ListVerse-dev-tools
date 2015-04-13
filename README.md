# ListVerse-dev-tools
Development tools for UCR ListVerse

Development
-----------
Install vagrant from [vagrantup.com](https://www.vagrantup.com/) and 
ansible via instructions found at [docs.ansible.com](http://docs.ansible.com/intro_installation.html) and run vagrant from this
directory.

Also, be sure to install [virtualbox](https://www.virtualbox.org/) as it acts as a driver for vagrant.

```sh
$ vagrant up
# Wait a while until box is provisioned
$ vagrant ssh
# Connect to the remote box
vagrant@vagrant-ubuntu-trusty-64:~$ . start_listverse.sh
# Sets up virtualenv and takes you to project directory
```
