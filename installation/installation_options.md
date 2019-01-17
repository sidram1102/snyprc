# Installation Options

You can install SNYPR using three different options:

- From the Snypr binary GUI installer 

If you want to install the application on Linux with GUI mode, and if X Window has not been configured, run these commands:

```sh
yum -y groupinstall "Desktop" "Desktop Platform" "X Window System" "Fonts"
yum install xorg-x11-xauth xterm
```