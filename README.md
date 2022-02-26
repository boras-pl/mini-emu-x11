# This is a set of helper scripts that allow you to run FS-UAE, DosBox and Vice C64 on minimal Debian with X11
Print this tutorial, seriously! Or open it on your smartphone, at least.

1. Download, burn and install any modern Debian netinst (Bullseye or daily) e.g. debian-testing-amd64-netinst.iso
2. Important! During installation an user MUST NOT be set to: emu, any other is allowed
- The 'emu' user is created automatically
- Install only standard system utilities. SSH is optional for remote administration.
- DO NOT install any windowing (Gnome, etc.) systems.
See attached screenshots if any doubts.
3. Boot and login as root
4. Execute following commands. You will be prompted for a password for the 'emu' user.
```
apt update
apt upgrade
apt install -y git
git clone https://github.com/boras-pl/mini-emu-x11.git
cd mini-emu-x11
./01_run_as_root.sh
```
