# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "precise64"

  config.vm.network :private_network, ip: "10.12.14.16"

  config.vm.provider "virtualbox" do |v|
    v.name = "devstack"
    v.customize ["modifyvm", :id, "--memory", "2048"]
    v.customize ["modifyvm", :id, "--cpuexecutioncap", "75"]
  end

end
