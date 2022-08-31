# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.synced_folder(
    "/Users/joelbandi/Devspace/dotfiles",
    "/home/vagrant/dotfiles",
    owner: "vagrant",
    group: "vagrant"
  )

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "4096"
  end
end
