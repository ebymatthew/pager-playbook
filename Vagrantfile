# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.box = "ubuntu/trusty64"
  # config.vm.box_check_update = false

  
  # If true, then any SSH connections made will enable agent forwarding.
  # Default value: false
  config.ssh.forward_agent = true
  config.ssh.forward_x11 = true

  config.vm.define "dev" do |c|
    c.vm.hostname = "dev"
    c.vm.network "private_network", ip: "192.168.100.2"
  end

  config.vm.define "master1" do |c|
    c.vm.hostname = "master1"
    c.vm.network "private_network", ip: "192.168.100.3"
  end

  config.vm.define "master2" do |c|
    c.vm.hostname = "master2"
    c.vm.network "private_network", ip: "192.168.100.4"
  end

  config.vm.define "master3" do |c|
    c.vm.hostname = "master3"
    c.vm.network "private_network", ip: "192.168.100.5"
  end

  config.vm.define "slave1" do |c|
    c.vm.hostname = "slave1"
    c.vm.network "private_network", ip: "192.168.100.6"
  end

  config.vm.define "slave2" do |c|
    c.vm.hostname = "slave2"
    c.vm.network "private_network", ip: "192.168.100.7"
  end
end
