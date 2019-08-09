# ansible-burner-laptop
Configures my burner laptop from a scratch Debian box. This typically happens before or during a security convention (DEFCON, CCC, etc.) and imagines all networks being hostile. It first install tor, and configures Debian to fetch all packages from their hidden service. It then upgrades the laptop to Debian Testing, and configures ufw, a firewall, to deny all incoming connections. Then it installs a bunch of useful packages for security conventions, including forensics tools, build utilities, and random utils (solarized tmux, curl, etc.)

## Usage
Clone this repo, then run:
```
sudo apt install ansible
sudo ./localhost.sh
```
