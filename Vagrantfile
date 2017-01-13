# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  # Set Vagrant box type
  config.vm.box = "ubuntu/trusty64"

  # Disable syncing of /vagrant folder
  config.vm.synced_folder ".", "/vagrant"

  # Run Ansible provisioner on ./provisioning/playbook.yml
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "provisioning/playbook.yml"
  end
end
