# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.network "private_network", ip: "192.168.50.4"
  config.vm.synced_folder "src/", "/vagrant"
  config.vm.provision :ansible do |ansible|
      ansible.playbook = "deploy/development/playbook.yml"
    end
end
