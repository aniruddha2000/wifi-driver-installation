# Installation guide of wifi driver in Ubuntu 18.04
---------------------------------------------------

### Install git

```
$ sudo apt update
$ sudo apt install git dkms
```

### Clone the repository

`$ git clone https://github.com/Mange/rtl8192eu-linux-driver.git`


### Build the driver software and install

```
$ sudo dkms add ./rtl8192eu-linux-driver
$ sudo dkms install rtl8192eu/1.0
```

### Blacklist the current driver

`$ echo "blacklist rtl8xxxu" | sudo tee /etc/modprobe.d/rtl8xxxu.conf`

### Reboot

`$ reboot`