Using Vagrant
- `vagrant init` - This allows you to create a new VM
- Go to the vagrantfile in the vagrant initialised directory
- edit the file to the version of Linux you want
- `Vagrant Up` - to "turn on" the VM
- `Vagrant SSH` - allows you to get into the machine

`sudo apt-get update -y` - Used to update the system
`sudo apt-get install nginx -y`- used to install ngins
`exit` - exit out of the VM
`vagrant reload` - exit out of the instance and reload the instance with new settings

`ps aux | grep nginx` - Shows running processes and services
