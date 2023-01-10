# DL-Setup-on-Ubunutu-20.04

This repo walks you through the steps that are needed for the installation of the Deep learning frameworks like PyTorch, Tensforflow on Ubuntu machine 20.04 LTS. 


> *Note : This setup guideline has been verified with the latest version of the  Ubunutu 22.04 LTS version*


## Tabel of contents

1. Ubuntu setup 
2. Install Cuda library
3. Install CudaNN
4. Install the DL frameworks 


-----------------------------------------------------------------------------------------

# Install ubuntu 20.04 LTS 

Firstly, download the Ubunutu OS image from the official website [link](https://releases.ubuntu.com/focal/ubuntu-20.04.5-desktop-amd64.iso). Then, flash the OS into bootable pen drive. You can use [Rufus](https://rufus.ie/en/) on windows or Startup disk creator on Ubuntu amchine to make a USB stick as pendrive. 

After installing the OS, run the folowing commands to update the OS. 


```
sudo apt update
sudo apt full-upgrade  --yes
sudo apt autoremove --yes
sudo apt autoclean --yes
reboot
```


## Install utility applications (optional)


###  Neofetch 

This is needed to get know the sytem's software and hardware details. With the hep of this library, we can get to know the GPU model name.  

   >	`sudo apt install neofetch`


### U Launcher 
Install the U launcher application to quickly navigate between the applications on Ubunutu.  


Install via PPA (Ubuntu): 
>`sudo add-apt-repository ppa:agornostal/ulauncher && sudo apt update && sudo apt install ulauncher`

## Install Google Chrome

Install google chrome browser
 
>`sudo dpkg -i <chrome-file-name.deb>`


## Install Anaconda

Anaconda simplifies the python packages / environments. The official website link to downdload the `.sh` file can be found [here](https://www.anaconda.com/products/distribution#linux)

```
# Navigate to the Downloads folder, 
CD ~/Downloads

# Firstly, install the dependencies 
apt-get install libgl1-mesa-glx libegl1-mesa libxrandr2 libxrandr2 libxss1 libxcursor1 libxcomposite1 libasound2 libxi6 libxtst6

# Dowload the and anaconda file(.sh file) and chehcksum from the official website's link. 
shasum -a Anaconda3-2022.10-Linux-x86_64.sh

# To install  the anaconda software, run the below command
bash ~/Downloads/Anaconda3-2022.10-Linux-x86_64.sh

```


