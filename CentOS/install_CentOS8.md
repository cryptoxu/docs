# Install CentOS Linux 8

## Install CentOS

1. download ISO images(http://isoredirect.centos.org/centos/8/isos/x86_64/CentOS-8.1.1911-x86_64-dvd1.iso)
2. start computer from ISO, select "Install CentOS Linux 8(default)"
3. language selection: English->English(United States)(default), continue
4. configuration:
	+ Installation Destination: Storage Configuration->Automatic(default)
	+ Network & Host Name: Ethernet -> On
	+ Software Selection: Server with GUI(default)
	then, click "Begin Installation"
5. during installation:
	+ click "Root Password" to set root password
	+ click "User Creation" to set user, check "Make this user administrator"
	after installation is completed, reboot
	
## Install teamviewer
1. open terminal: Activities->Terminal
2. in bash,execute commands:
	+ sudo dnf -y install https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm
	+ sudo dnf -y install wget
	+ wget https://download.teamviewer.com/download/linux/teamviewer.x86_64.rpm
	+ sudo dnf --enablerepo epel-playground install ./teamviewer.x86_64.rpm
3. start teamviewer by: Activities->Show Application->Teamviewer, after teamviewer GUI shown, record "Your ID" and "Password" fields