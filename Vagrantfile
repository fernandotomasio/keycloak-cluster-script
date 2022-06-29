# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/bionic64"


  config.vm.define "postgresql" do |m|
    m.vm.network "private_network", ip: "192.168.56.10"  
  end

  config.vm.define "nginx-reverse-proxy" do |m|
    m.vm.hostname = "nginx-reverse-proxy"
    m.vm.network "private_network", ip: "192.168.56.11"  
  end

  config.vm.define "keycloak-server1" do |m|
    m.vm.hostname = "keycloak-server"
    m.vm.network "private_network", ip: "192.168.56.12"  
  end

  config.vm.define "keycloak-server2" do |m|
    m.vm.hostname = "keycloak-server"
    m.vm.network "private_network", ip: "192.168.56.13"  
  end

  config.vm.define "keycloak-server3" do |m|
    m.vm.hostname = "keycloak-server"
    m.vm.network "private_network", ip: "192.168.56.14"  
  end
 
end
