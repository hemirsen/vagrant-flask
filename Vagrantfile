# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.network "forwarded_port", guest: 5000, host: 5000
    config.vm.provider "docker" do |d|
        d.image = "g181210038/flaskapp:latest"
        d.name = "flaskapp"
    end
end