# -*- mode: ruby -*-
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"

  config.vm.define "webserver" do |webserver|
    webserver.vm.network "private_network", ip: "192.168.10.100"
    webserver.vm.hostname = "server"
    webserver.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
    end
  end
end