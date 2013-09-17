# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "centos-6_4-64_percona"
  config.vm.box_url = "https://my.bitcasa.com/download-send/d5827f41b88f83bd8846c90314d5387551902764a3edc8d32e79e847d30e1ebc/f416a60a0479a0bd94f814cb5f19ab87c05aa9eb3d4afb24597ccd55ec3a30cc/centos-6_4-64_percona_virtualbox.box"

  config.ssh.username = "root"

  config.vm.define "node1" do |node1|
    node1.vm.hostname = 'node1'
    node1.vm.network :private_network, ip: '192.168.70.2'
  end

  config.vm.define "node2" do |node2|
    node2.vm.hostname = 'node2'
    node2.vm.network :private_network, ip: '192.168.70.3'
  end
end
