# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
config.vm.box = "debian/jessie64"
 config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.inventory_path = "hosts"
    ansible.playbook = "set_ansible.yml"  
    ansible.limit = "all" #https://github.com/jlund/mazer-rackham/issues/7

 end
end
