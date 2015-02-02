# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.define "arch" do |arch|
    arch.vm.box = "terrywang/archlinux"

    arch.vm.provision "ansible" do |ansible|
        ansible.playbook = "Vagrantplaybook.yml"
        ansible.extra_vars = {
            ansible_python_interpreter: "/usr/bin/python2",
        }
    end
  end
end
