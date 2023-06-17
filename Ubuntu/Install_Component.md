## Install Chrome By Command Line
```bash
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i google-chrome-stable_current_amd64.deb
```
## Install Git
```bash
sudo apt install git -y
```
## Install & Uninstall Brew
```bash
sudo apt update
sudo apt-get install build-essential
sudo apt install git -y
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
(echo; echo 'eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"') >> /home/$USER/.bashrc
eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
brew doctor
brew install gcc
# uninstall
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/uninstall.sh)"
```

## Install NVM
```bash
sudo apt install curl 
curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
source ~/.bashrc   
nvm install node 
nvm install 12
nvm install --lts 
nvm list
nvm use default 12
nvm run default --version 
# uninstall
nvm uninstall 18.16.0 
```


