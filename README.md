# Final Year Project: Visualising Software Defined-Networking using Ryu and Mininet

## Project Paper
You can view it at this [Google Drive link](https://drive.google.com/open?id=10VTDsbn1Uk7HXbeOAyGF5RuovBKkp16w)

## Explanation Slides
You can view it at this [Google Drive link](https://drive.google.com/file/d/1-Y2Dm2jJJi_xTyYHcp-0HjGHjkUTdzNx/view?usp=sharing)

## My Software-Defined Network(along with other setups completed)
You can get it at this [Google Drive link](https://drive.google.com/file/d/1-biQrQG8MhXaX6VorSlmGy73LYzEw2DN/view?usp=sharing).

## Demo Videos
1. [Simple Web Server and Client](https://drive.google.com/file/d/1-2x9P_S8ENII0ebv8rNZXTGJJN821pCn/view?usp=sharing)
2. [Simulating Switching Hub](https://drive.google.com/file/d/1-Jwpa_zM4bTpd0A5qErpwvrHhG1s2-oH/view?usp=sharing)
3. [Interact with Ryu using Postman](https://drive.google.com/drive/folders/103odq5cu5m8F4rEcoqq1UBuiXXfbV3t_?usp=sharing)
4. [Ryu with Flow Manager](https://drive.google.com/drive/folders/1-qKCp7tPDSw1XyXv0CKIRcZGD4vJZs56?usp=sharing)
5. [Experimenting with VLAN](https://drive.google.com/drive/folders/1-ioIH_r7RlPOqjDWDSgKFZR8YrC0rdso?usp=sharing)
6. [Simple performance measurement experimentation](https://drive.google.com/file/d/1-FfxqqrOPyv2RLDwuQZpkrcBLWKX1Md0/view?usp=sharing)

## Setting up network test bed for Software-Defined Networking(If you want to set it up yourself)

### Hardware
My machine general specifications: 
- Intel Core i5 Dual-Core @ 1.70 GHz (2GHz or more is recommended)
- 4GB of RAM(8GB is recommended because virtualization takes a lot of computer resources)

I use Windows so I need to set up below software before I start other installation as stated below:

### Software

* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Xming X Server](https://sourceforge.net/projects/xming/)
* [PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

### Other
#### [Ubuntu](https://ubuntu.com/download/desktop)
I use Ubuntu Server 16.04.3 LTS but you can use whatever Ubuntu version you have from 14, or 18. It is however recommended to use Ubuntu 16 or 18 only because the older 14 or the latest one, 19 may have some problems while installing Ryu SDN framework. If you're not familiar with the server version which are simple and light, then you can use the desktop version.

##### __Setting up VM__
Follow this [wiki on set up virtual machine](https://github.com/mininet/openflow-tutorial/wiki/Set-up-Virtual-Machine#Finish_VM_Setup)

##### __Setting up Network Access__
Follow this [wiki on set up network access](https://github.com/mininet/openflow-tutorial/wiki/Set-up-Virtual-Machine#Set_Up_Network_Access)

#### [Mininet](http://mininet.org/)
I use [native installation from source](http://mininet.org/download/#option-2-native-installation-from-source) since it's the better way to get start developing.

#### [Ryu](https://osrg.github.io/ryu/)
Make sure you have python and pip installed already. On Ubuntu 16.04 LTS and later, make sure [ryu dependencies](https://ryu.readthedocs.io/en/latest/getting_started.html#prerequisites) required are installed,  before you install Ryu. The easiest way is by pip command. _pip install python3-ryu or python-ryu_ if ryu-manager can't run after installing with normal _pip install ryu_. You can try this [way](https://github.com/andrew-miao/study_sdn/tree/master/install) too if you still encounter problem installing it. Lastly, try install from source code if installing from a package manager still not successful.

#### [Pox](https://github.com/noxrepo/pox)
If you have installed Mininet, Pox controller already included along with it.

#### [Postman](https://www.getpostman.com/downloads/)
If you are using Ubuntu Server, you may need to install it the other way by installing the basic GUI to the server itself and run Postman from there by following this [wiki on running a GUI in the VM console window](https://github.com/mininet/openflow-tutorial/wiki/Set-up-Virtual-Machine#Alternative_Run_a_GUI_in_the_VM_console_window).

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/gEyu8nnDYyo/0.jpg)](http://www.youtube.com/watch?v=gEyu8nnDYyo) 


#### [FlowManager](https://github.com/martimy/flowmanager)
It can be installed by git clone the repository.

#### Firefox
If you use GUI-based Ubuntu version, it's probably pre-installed already and if not, then you need to install it through the package manager. If you are using Ubuntu Server and have not installed the X11 itself and a windows manager, flwm or lxde, you can by follow this [wiki on running a GUI in the VM console window](https://github.com/mininet/openflow-tutorial/wiki/Set-up-Virtual-Machine#Alternative_Run_a_GUI_in_the_VM_console_window). After that, doing _sudo apt-get install firefox_ will install ffox and its dependencies, as well as a runtime environment
