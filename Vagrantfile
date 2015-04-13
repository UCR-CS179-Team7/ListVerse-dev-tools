# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  # environment is Ubuntu v14.04
  config.vm.box = "ubuntu/trusty64"

  # accessing "localhost:8080" will access port 80 on the guest machine.
  config.vm.network "forwarded_port", guest: 80, host: 8080

  # Sync the main project folder with /opt/ListVerse
  config.vm.synced_folder "../", "/opt/ListVerse"

  config.vm.provider "virtualbox" do |vb|
    # Customize the amount of memory on the VM:
    vb.memory = "1024"
  end

  # use Ansible as a provisioner
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "site.yml"
  end
end
