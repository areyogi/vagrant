# -*- mode: ruby -*-
# vi: set ft=ruby :
 
# Configuration Parameters
UBUNTU_VBOX="ubuntu-xenial64-20190918.0.0"
BASEBOX_NAME="yogesh_box"

Vagrant.configure("2") do |config|
  config.vm.box = UBUNTU_VBOX

  config.vm.provider "virtualbox" do |v|
    v.name = BASEBOX_NAME
  end

  # consciously go to a specific version if need be.
  config.vm.box_check_update = false

  # Provision the VM by running the installation script
  config.vm.provision "shell", inline: <<-SHELL
    cd /vagrant
    echo "everything is  fine"
  SHELL
end