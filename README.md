# HOW TO INSTALL SUBLIME TEXT 3
 ## IN WINDOWS 
 1. For [Windows](https://download.sublimetext.com/Sublime%20Text%20Build%203211%20Setup.exe)
 2. For [Windows 64 bit](https://download.sublimetext.com/Sublime%20Text%20Build%203211%20x64%20Setup.exe)
 
 ## IN LINUX
   1. For [DEB](https://download.sublimetext.com/sublime-text_build-3211_amd64.deb) 
   2. For [RPM](https://download.sublimetext.com/sublime-text-3211-1.x86_64.rpm)
   3. For [pkg.tar.xz](https://download.sublimetext.com/sublime-text-3211-1-x86_64.pkg.tar.xz)
   4. For [64bit tar](https://download.sublimetext.com/sublime_text_3_build_3211_x64.tar.bz2)
   5. For [32bit tar](https://download.sublimetext.com/sublime_text_3_build_3211_x32.tar.bz2)

## Whats New
  ![image](https://user-images.githubusercontent.com/67573209/143979275-e66e476f-4c03-4300-b4bd-c567592a1b87.png)



### FOR DEB 
    sudo dpkg -i <sublime deb file>

### IN LINUX USING TERMINAL
   ##### INSTALLATION  
    wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
    echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
    sudo apt update
    sudo apt install sublime-text
    
### UNINSTALL 
    sudo apt-get remove sublime-text
    sudo apt-get autoremove



#### NEW SUBLIME MERGE (GIT CLIENT)
  1. [WINDOWS](https://www.sublimemerge.com/download_thanks?target=win-x64)
  ##### Linux
  #### apt
The apt repository contains packages for both x86-64 and arm64.

Install the GPG key:
        
        wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -

Ensure apt is set up to work with https sources:

        sudo apt-get install apt-transport-https

##### Select the channel to use:

Stable
      
    echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
Dev

    echo "deb https://download.sublimetext.com/ apt/dev/" | sudo tee /etc/apt/sources.list.d/sublime-text.list

Update apt sources and install Sublime Merge

    sudo apt-get update
    sudo apt-get install sublime-merge
  
  #### pacman
Install the GPG key:

    curl -O https://download.sublimetext.com/sublimehq-pub.gpg && sudo pacman-key --add sublimehq-pub.gpg && sudo pacman-key --lsign-key 8A8F901A && rm sublimehq-pub.gpg

Select the channel to use:

Stable x86_64

    echo -e "\n[sublime-text]\nServer = https://download.sublimetext.com/arch/stable/x86_64" | sudo tee -a /etc/pacman.conf
Dev x86_64

    echo -e "\n[sublime-text]\nServer = https://download.sublimetext.com/arch/dev/x86_64" | sudo tee -a /etc/pacman.conf
Stable aarch64

    echo -e "\n[sublime-text]\nServer = https://download.sublimetext.com/arch/stable/aarch64" | sudo tee -a /etc/pacman.conf
Dev aarch64

    echo -e "\n[sublime-text]\nServer = https://download.sublimetext.com/arch/dev/aarch64" | sudo tee -a /etc/pacman.conf
Update pacman and install Sublime Merge

    sudo pacman -Syu sublime-merge
  #### yum
Install the GPG key:

    sudo rpm -v --import https://download.sublimetext.com/sublimehq-rpm-pub.gpg
Select the channel to use:

Stable
    
    sudo yum-config-manager --add-repo https://download.sublimetext.com/rpm/stable/x86_64/sublime-text.repo
Dev

    sudo yum-config-manager --add-repo https://download.sublimetext.com/rpm/dev/x86_64/sublime-text.repo
Update yum and install Sublime Merge

    sudo yum install sublime-merge
Note there are no RPM packages for ARM currently.

  #### dnf
Install the GPG key:

    sudo rpm -v --import https://download.sublimetext.com/sublimehq-rpm-pub.gpg
Select the channel to use:

Stable
    
    sudo dnf config-manager --add-repo https://download.sublimetext.com/rpm/stable/x86_64/sublime-text.repo
Dev
    
    sudo dnf config-manager --add-repo https://download.sublimetext.com/rpm/dev/x86_64/sublime-text.repo
Update dnf and install Sublime Merge

    sudo dnf install sublime-merge
Note there are no RPM packages for ARM currently.

  #### zypper
Install the GPG key:

    sudo rpm -v --import https://download.sublimetext.com/sublimehq-rpm-pub.gpg
Select the channel to use:

Stable
    
    sudo zypper addrepo -g -f https://download.sublimetext.com/rpm/stable/x86_64/sublime-text.repo
Dev

    sudo zypper addrepo -g -f https://download.sublimetext.com/rpm/dev/x86_64/sublime-text.repo
Update zypper and install Sublime Merge

    sudo zypper install sublime-merge
Note there are no RPM packages for ARM currently.
