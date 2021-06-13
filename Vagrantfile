# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.provision "shell", path: "provision-docker.sh"
  
  config.vm.network "forwarded_port", guest: 27000, host: 27000
  config.vm.provider "virtualbox" do | vb |
    vb.memory = 1024
    vb.cpus = 1
  end

end
