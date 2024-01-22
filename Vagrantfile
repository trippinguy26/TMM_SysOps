# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/jammy64"
  config.vm.network "public_network", type: "dhcp"
  config.vm.provision "shell", path: "install-docker.sh"
  config.vm.provision "shell", path: "run-docker-compose.sh"
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "4096"
    vb.cpus = "2"
  end
end
