# Final Year Project: Visualising Software Defined-Networking using Ryu and Mininet

## Setting up network test bed for Software-Defined Networking

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
Follow this [guide][https://github.com/mininet/openflow-tutorial/wiki/Set-up-Virtual-Machine#Finish_VM_Setup]

##### __Setting up Network Access__
Follow this [guide][https://github.com/mininet/openflow-tutorial/wiki/Set-up-Virtual-Machine#Set_Up_Network_Access]

#### [Mininet](http://mininet.org/)
I use http://mininet.org/download/#option-2-native-installation-from-source since it's the better way to get start developing.

#### [Ryu](https://osrg.github.io/ryu/)
Make sure you have python and pip installed already. On Ubuntu 16.04 LTS and later, make sure the [dependencies][https://ryu.readthedocs.io/en/latest/getting_started.html#prerequisites] required are installed,  before you install Ryu. The easiest way is by pip command. _pip install python3-ryu or python-ryu_ if ryu-manager can't run after installing with normal _pip install ryu_. You can try this [way][https://github.com/andrew-miao/study_sdn/tree/master/install] too if you still encounter problem installing it. Lastly, try install from source code if installing from a package manager still not successful.

#### [Pox](https://github.com/noxrepo/pox)
If you have installed Mininet, Pox controller already included along with it.

#### [Postman](https://www.getpostman.com/downloads/)
If you are using Ubuntu Server, you may need to install it the other way https://www.youtube.com/watch?v=gEyu8nnDYyo. If you have problem executing Postman by SSH session with Xming server running, you may need to install the basic GUI to the server itself and run Postman from there by following this https://github.com/mininet/openflow-tutorial/wiki/Set-up-Virtual-Machine#Alternative_Run_a_GUI_in_the_VM_console_window

#### [FlowManager](https://github.com/martimy/flowmanager)
It can be installed by git clone the repository.

#### Firefox
If you use GUI-based Ubuntu version, it's probably pre-installed already and if not, then you need to install it through the package manager. Since I am using Ubuntu Server which is not GUI, I have installed X11 itself and a windows manager, flwm by following this [guide][https://github.com/mininet/openflow-tutorial/wiki/Set-up-Virtual-Machine#Alternative_Run_a_GUI_in_the_VM_console_window]. After that, doing _sudo apt-get install firefox_ will install ffox and its dependencies, as well as a runtime environment
