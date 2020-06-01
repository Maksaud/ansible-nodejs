# -*- mode: ruby -*-
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"

  config.vm.define "webserver" do |webserver|
    webserver.vm.hostname = "server"
    webserver.vm.provision "ansible" do |ansible|
      ansible.playbook = "playbook.yml"
    end
  end
end