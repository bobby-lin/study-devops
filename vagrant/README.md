# Vagrant Basics

## Installation
Download Vagrant installer for your chosen OS:
https://developer.hashicorp.com/vagrant/downloads

Install VirtualBox: https://www.virtualbox.org/wiki/Downloads

## Creating a VM
Create a `Vagrantfile`:
```text
Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/bionic64"
  config.vm.box_version = "1.0.282"
end
```

Run:
```console
vagrant up --provider virtualbox
```

## SSH into the machine

Run:
```console
vagrant ssh
```
