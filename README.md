# Installation guide of wifi driver in Ubuntu 16.04
--------------------------------------------

### Install git

```
$ sudo apt update
$ sudo apt install git
```

### Clone the repository

`$ git clone https://github.com/jeremyb31/rtl8192eu-linux-driver`

### Navigate to the directory of the driver

`$ cd rtl8192eu-linux-driver`

### Build the driver software and install

```
$ make
$ sudo make install
```

### Reboot

`$ reboot`
