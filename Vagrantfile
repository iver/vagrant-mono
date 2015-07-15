# -*- mode: ruby -*-
# # vi: set ft=ruby :
#
# # Vagrantfile API/syntax version. Don't touch unless you know what you're doing!

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box_url = "https://atlas.hashicorp.com/ARTACK/boxes/debian-jessie"
  config.vm.box = "ARTACK/debian-jessie"
  config.vm.network "private_network", ip: "10.2.2.203"
  config.vm.provision :shell, path: "bin/setup.sh"

  config.ssh.forward_agent = true

  config.vm.provider "virtualbox" do |vb|
    vb.customize [ "guestproperty", "set", :id, "/VirtualBox/GuestAdd/VBoxService/--timesync-set-threshold", 10000 ]
    vb.gui = true
    vb.memory = 1024
    vb.cpus = 2
  end
end
