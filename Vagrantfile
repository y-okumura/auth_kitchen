# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-6.7"

  config.vm.define :RP do |proxy|
    proxy.vm.network "private_network", ip: "192.168.33.10"
  end

  config.vm.define :SSO do |sso|
    sso.vm.network "private_network", ip: "172.16.33.11"
  end

  config.vm.define :LDAP do |sso|
    sso.vm.network "private_network", ip: "172.16.33.12"
  end
end
