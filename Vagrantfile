# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "CentOS65_ansible"
  config.vm.box_url = "https://github.com/2creatives/vagrant-centos/releases/download/v6.5.3/centos65-x86_64-20140116.box"

  # network
  config.vm.network "private_network", ip:"172.17.5.100"
  config.vm.hostname="neo4j.local"

  #syncee
  config.vm.synced_folder "./", "/vagrant", disabled: true

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook/vagrant.yml"
  end
end
