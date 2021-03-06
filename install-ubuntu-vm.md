## Install an Ubuntu Linux virtual machine on your Macbook:

* You'll need about 10GB free disk space for this to work.
* Download and install Virtualbox from https://www.virtualbox.org/wiki/Downloads (OS X Hosts)
* Download and install Vagrant from https://www.vagrantup.com/downloads.html (MacOS 64-bit)
* Make a directory to build your vm in, and a subdirectory to be shared between the vm and your mac:
```bash
$ mkdir ~/ubuntu
$ cd ~/ubuntu
$ mkdir shared

```

* Download ubuntu-18.04-server.box and Vagrantfile from  https://drive.google.com/open?id=0B7wMY76wVokRa3hqOFFjVG9ETms and move those two files to the directory you just made.
* Now use Vagrant to build and start your virtual machine:
```bash
$ vagrant box add --name ubuntu-server ./ubuntu-18.04-server.box
$ vagrant up
```
* If everything went well, you can now log into your new virtual machine:
```bash
$ vagrant ssh
```
This should give you a shell prompt on your vm:
```bash
vagrant@ubuntu:~/
```
On my machine it's green :-)

* Congratulations, you're now logged in to your Ubuntu virtual machine.
   * You are logged in as the `vagrant` user with `sudo` access, so you can do whatever you like.
   * You should have a subdirectory called `shared` in the vagrant home directory.  This is a mount of `~/ubuntu/shared` on your mac, so files you create in one place should magically appear in the other. 
   * Python3 and Git are already installed.  Knock yourself out!

* When you're done, you can type `exit` to close your session on the vm.  Back at the MacOS shell prompt, you can type:
```bash
$ vagrant halt
```
to stop the virtual machine from running in the background.  Whenever you like, you can restart the vm and log in like this:
```bash
$ cd ~/ubuntu
$ vagrant up
$ vagrant ssh
```






