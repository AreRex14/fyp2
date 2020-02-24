# Final Year Project: Visualising Software Defined-Networking using Ryu and Mininet

## Hardware & Software Installation

### Hardware
My PC general specifications: Intel Core i5 Dual-Core 1.70 GHz with 4GB of RAM(8GB and better processor speed is recommended because virtualization takes a lot of your computer resources)

I use Windows so I need to set up below software before I start other installation as stated below:

### Software

* VirtualBox https://www.virtualbox.org/wiki/Downloads
* Xming X Server https://sourceforge.net/projects/xming/
* PuTTY https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html

### Other
Ubuntu https://ubuntu.com/download/desktop
In my case, I use Ubuntu Server 16.04.3 LTS but you can use whatever Ubuntu version you have from 14, or 18. I recommend you to use the desktop version if you're not familiar with server but server is simple and light, suited to what I'll only be doing which is the project.

__Setting up VM__
Select your VM and go to the Settings Tab. Go to Network->Adapter 2. Select the "Enable adapter" box, and attach it to "host-only network".(Sidenote: on a new VirtualBox installation you may not have any "host-only network" configured yet. To have one select Global Tools -> Host Network Manager -> create or File -> Host Network Manager -> create. Click create with default settings. Then you can try the attach.) This will allow you to easily access your VM through your host machine.

At that point you should be ready to start your VM. Press the "Start" arrow icon or double-click your VM within the VirtualBox window. 

__Setting up Network Access__
You should make sure your VM has two network interfaces. One should be a NAT interface that it can use to access the Internet, and the other should be a host-only interface to enable it to communicate with the host machine. For example, your NAT interface could be eth0 and have a 10.x IP address, and your host-only interface could be eth1 and have a 192.168.x IP address. You should ssh into the host-only interface at its associated IP address. Both interfaces should be configured using DHCP. If they are not already configured, you may have to run dhclient on each of them, as described below.

For more detailed instructions, see VirtualBox Specific Instructions. 

Mininet http://mininet.org/
I use http://mininet.org/download/#option-2-native-installation-from-source since it's the better way to get start developing.

Ryu https://osrg.github.io/ryu/
Make sure you have python and pip installed already. On Ubuntu 16.04 LTS and later, make sure the dependencies required are installed, https://ryu.readthedocs.io/en/latest/getting_started.html#prerequisites before you install it. The easiest way is by pip command but if you encounter problem, try install it from source code. You can try this way too https://github.com/andrew-miao/study_sdn/tree/master/install if you still encounter problem installing it from the simple way.

Postman https://www.getpostman.com/downloads/
If you are using Ubuntu Server, you may need to install it the other way https://www.youtube.com/watch?v=gEyu8nnDYyo. If you have problem executing Postman by SSH session with Xming server running, you may need to install the basic GUI to the server itself and run Postman from there by following this https://github.com/mininet/openflow-tutorial/wiki/Set-up-Virtual-Machine#Alternative_Run_a_GUI_in_the_VM_console_window
