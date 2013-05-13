# Marconi

An easy-to-use [Vagrant](http://docs.vagrantup.com/v2/)-based setup for GNU Radio applications.

## Usage

First, download and install the latest version of Vagrant from [http://downloads.vagrantup.com](http://downloads.vagrantup.com). Do not count on your package manager to deliver the latest version of Vagrant.

Once Vagrant is set up:

```bash
$ git clone git://github.com/yuvadm/marconi.git && cd marconi
$ vagrant up
```

Initially running `vagrant up` will take a while since Vagrant will need to download the initial virtual machine, and then proceed to install all the dependencies, and compile GNU Radio. After all these steps are through, you should have a fully working GNU Radio environment running on an Ubuntu virtual machine. SSH into the machine with:

```bash
$ vagrant ssh
```

Halt or destroy the instance with:

```bash
$ vagrant [halt|destroy]
```

## License and Credits

Marconi is released under the [GPLv3](http://www.gnu.org/licenses/gpl-3.0.txt) license.

Created by Yuval Adam, based on the [`build-gnuradio`](http://www.sbrac.org/files/build-gnuradio) script by Marcus Leech.
