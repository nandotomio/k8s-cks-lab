# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-20.04-arm64"

  config.vm.define "control_plane" do |control_plane|
    control_plane.vm.hostname = "control_plane"
    control_plane.vm.network "private_network", ip: "10.10.10.11"
    control_plane.vm.provider "parallels" do |prl|
      prl.name = "control_plane"
      prl.memory = 4096
      prl.cpus = 2
    end  
  end

  config.vm.define "node1" do |node1|
    node1.vm.hostname = "node1"
    node1.vm.network "private_network", ip: "10.10.10.12"
    node1.vm.provider "parallels" do |prl|
      prl.name = "node1"
      prl.memory = 4096
      prl.cpus = 2
    end
  end
end
