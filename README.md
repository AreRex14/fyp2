Final Year Project: Visualising Software Defined-Networking using Ryu and Mininet

Hardware & Software Installation

Hardware
My PC general specifications: Intel Core i5 Dual-Core 1.70 GHz with 4GB of RAM(8GB and better processor speed is recommended because virtualization takes a lot of your computer resources)

I use Windows so I need to set up below software before I start other installation as stated below:

Software

VirtualBox https://www.virtualbox.org/wiki/Downloads
Xming X Server https://sourceforge.net/projects/xming/
PuTTY https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html

Other
Ubuntu https://ubuntu.com/download/desktop
In my case, I use Ubuntu Server 16.04.3 LTS but you can use whatever Ubuntu version you have from 14, or 18. I recommend you to use the desktop version if you're not familiar with server but server is simple and light, suited to what I'll only be doing which is the project.

Setting up VM


Mininet http://mininet.org/
I use http://mininet.org/download/#option-2-native-installation-from-source since it's the better way to get start developing.

Ryu https://osrg.github.io/ryu/
Make sure you have python and pip installed already. On Ubuntu 16.04 LTS and later, make sure the dependencies required are installed, https://ryu.readthedocs.io/en/latest/getting_started.html#prerequisites before you install it. The easiest way is by pip command but if you encounter problem, try install it from source code. You can try this way too https://github.com/andrew-miao/study_sdn/tree/master/install if you still encounter problem installing it from the simple way.

Postman https://www.getpostman.com/downloads/
If you are using Ubuntu Server, you may need to install it the other way https://www.youtube.com/watch?v=gEyu8nnDYyo. If you have problem executing Postman by SSH session with Xming server running, you may need to install the basic GUI to the server itself and run Postman from there by following this https://github.com/mininet/openflow-tutorial/wiki/Set-up-Virtual-Machine#Alternative_Run_a_GUI_in_the_VM_console_window
