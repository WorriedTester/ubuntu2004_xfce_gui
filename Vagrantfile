# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  
  # Ubuntu 20.04 https://app.vagrantup.com/ubuntu/boxes/focal64
  config.vm.box = "ubuntu/focal64"

  # Provider-specific configuration
  config.vm.provider "virtualbox" do |vb|
    # Customize the amount of processors, assigned to this VM
    vb.cpus = 1

    # Customize the amount of memory on the VM
    vb.memory = "2048"
  end

  config.vm.provision "shell", inline: <<-SHELL
    export DEBIAN_FRONTEND=noninteractive
    apt-get update
    apt-get install -y xfce4
  SHELL
end
