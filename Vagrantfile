# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.ssh.insert_key = false
  
  config.vm.define "mysql1" do |mysql|
    mysql.vm.box = "centos/7"
    mysql.vm.hostname = "mysql1"
    mysql.vm.network "private_network", ip: "192.168.0.7"
    mysql.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.memory = 1024
    end
  end
end