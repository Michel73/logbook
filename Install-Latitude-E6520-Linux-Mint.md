# DELL Latitude E6520 with Linux Mint

# 2015-01-30
* Installed Linux Mint 17.1 Cinnamon
* F12 -> enable UEFI boot
* Graphic card problems on second monitor (multiple mouse symbols)
* NVIDIA Corporation: GF119M [NVS 4200M] - use nvidia-331 driver Version 331.113-0ubuntu0.0.4
* Installed dotfiles
```bash
sudo apt-get install git
mkdir code && cd code
git clone https://github.com/StefanScherer/dotfiles && cd dotfiles && ./sync.sh
sudo apt-get install vim
```
* Downloaded and installed Vagrant 1.7.2
```bash
sudo apt-get install virtualbox-4.3
vagrant plugin install vagrant-cucumber
vagrant plugin install vagrant-multiprovider-snap
vagrant plugin install vagrant-pristine
sudo apt-get install curl
```
* Install GVM
```bash
bash < <(curl -L -s https://raw.github.com/moovweb/gvm/master/binscripts/gvm-installer)
sudo apt-get install mercurial bison
gvm install go1.3
gvm use go1.3 --default
```
