# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "centos/8"
  config.vm.synced_folder ".", "/vagrant", type: "virtualbox"
  config.vm.hostname = "1day.local"
  config.vm.network :private_network, ip: "192.168.56.50"
  config.vm.provider :virtualbox do |vb|
    vb.name = "1day"
    vb.customize ["modifyvm", :id, "--memory", "768"]
  end
end