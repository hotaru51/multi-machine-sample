# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  # config.vm.network "private_network", type: "dhcp"

  config.vm.define "machine_a" do |machine|
    machine.vm.network "private_network", ip: "192.168.1.101"
  end

  config.vm.define "machine_b" do |machine|
    machine.vm.network "private_network", ip: "192.168.1.102"
  end

  config.vm.provider "virtualbox" do |vb|
    # Display the VirtualBox GUI when booting the machine
    vb.gui = false
  
    # Customize the amount of memory on the VM:
    vb.memory = "2048"
    vb.cpus = "1"
  end
end
