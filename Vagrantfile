# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "chef/centos-7.0"
  config.vm.define "node1" do |node1|
    node1.vm.network "private_network", ip: "192.168.33.10"
    node1.vm.hostname = "node1"
    node1.vm.box = "mesos-master"
  end

  config.vm.define "node2" do |node2|
    node2.vm.network "private_network", ip: "192.168.33.11"
    node2.vm.hostname = "node2"
  end
end
