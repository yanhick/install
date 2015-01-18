# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.define "install" do |install|
      install.vm.box = "ubuntu/trusty64"
      install.vm.hostname = "install"
      install.vm.provision "ansible" do |ansible|
          ansible.playbook = "install.yml"
      end
  end
end
