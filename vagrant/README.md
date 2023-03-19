# Vagrant Basics

## Installation
Download Vagrant installer for your chosen OS:

https://developer.hashicorp.com/vagrant/downloads

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
vagrant up --provider hyperv
```

## SSH into the machine

Run:
```console
vagrant ssh
```
