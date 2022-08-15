# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define "server1" do |server1|
    server1.vm.box = "ubuntu/bionic64"
    server1.vm.disk :disco, nome: "Storage", tamanho: "20GB"
    server1.vm.network "private_network", ip: "10.10.10.11"
    server1.vm.network "public_network", ip: "192.168.15.100"
    server1.vm.hostname = "devops.local"
  end
  config.vm.define "server2" do |server2|
    server2.vm.box = "ubuntu/bionic64"
    server2.vm.disk :disco, nome: "Storage", tamanho: "30GB"
    server2.vm.network "public_network", ip: "192.168.15.101"
    server2.vm.network "private_network", ip: "10.10.10.12"
    server2.vm.hostname = "IaC.local"
  end
end

