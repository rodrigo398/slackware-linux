# Slackware - Linux
In this repo, we are gonna try to provide a handful of commands to set up our Slackware environment.


#### Post Installation
useradd -d /home/rodrix -c "rodrix" -m -s /bin/bash rodrix

passwd rodrix

usermod -g wheel rodrix

visudo

useradd -m -g users -G floppy,audio,video,cdrom,plugdev,power,netdev,lp,scanner -s /bin/bash rodrix

usermod -G floppy,audio,video,cdrom,plugdev,power,netdev,lp,scanner -a rodrix


vim /etc/inittab

vim /etc/lilo.conf


#### Install Google Chrome from RPM

rpm2tgz google-chrome-stable_current_x86_64.rpm


#### Install Slpkg

tar xvf slpkg-3.8.5.tar.gz 

cd slpkg-3.8.5

./install.sh 

#### How to install different apps?

Install vscode, discord, slack from RPM.

Install teamviewer from slonl 

Install skype from DEB 

Install VirtualBox from .run file 


#### Memory VSCode
echo fs.inotify.max_user_watches=524288 | tee -a /etc/sysctl.conf
