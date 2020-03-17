# Vagrant and Virtualbox

Setting up and learning about a basic virtual machine

## Vagrant
This allows us to manage and provision virtual machines. It also allows us to pull images of VMs from its marketplace.

## Virtualbox
This is the software that does all the heavy lifting of creating said VMs

Using Vagrant
- `vagrant init` - This allows you to create a new VM
- Go to the vagrantfile in the vagrant initialised directory
- edit the file to the version of Linux you want
- `Vagrant Up` - to "turn on" the VM
- `Vagrant SSH` - allows you to get into the machine

`sudo apt-get update -y` - Used to update the system
`sudo apt-get install nginx -y`- used to install nginx
`exit` - exit out of the VM
`vagrant reload` - exit out of the instance and reload the instance with new settings

`ps aux | grep nginx` - Shows running processes and services

## Within the vagrantfile

```ruby
config.vm.box = "ubuntu/bionic64"
config.vm.network "private_network", ip: '192.168.10.100'
```
The first line tells Vagrant what OS you wish to install.
The second line tells Vagrant how to configur the network. Entering the IP into the web browser allows you to access the file.
