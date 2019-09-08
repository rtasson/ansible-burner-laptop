# ansible-burner-laptop
Configures a burner laptop from a base Debian box. This typically happens before or during a security convention (DEFCON, CCC, etc.) and imagines all networks being hostile.

It does a couple of things:
* installs Tor and sets the default apt repositories to point to Debian's hidden service
* upgrades Debian to Testing
* some basic hardening, including installing UFW, uninstalling noisy networking packages & installs apparmor
* installs a bunch of utilities - wireguard, build utils, forensics utils, solarized tmux

## Usage
Clone this repo, then run:
```
sudo apt install ansible
sudo ./localhost.sh
```

## todo
* create a firefox apparmor profile
* further hardening - but what??
* get wireguard a bit more configured - create interface
