Vagrant Wnd-Chrm:
-------------
A stack configuration for Vagrant containing wnd-chrm, an image analysis application.  For more information
on wnd-chrm see the wnd-chrm documentation [here](https://github.com/wnd-charm/wnd-charm).

Installation:
-------------

Download and install [VirtualBox](http://www.virtualbox.org/)

Download and install [vagrant](http://vagrantup.com/)

Download a vagrant box (name of the box is supposed to be precise64)

    $ vagrant box add precise64 http://files.vagrantup.com/precise64.box

Clone this repository

Go to the repository folder and launch the box

    $ cd [repo]
    $ vagrant up

What's inside:
--------------

Installed software:

* C++ Compiler (build-essential)
* X11 libraries (libX11-dev, libxt-dev, libxaw7-dev)
* [LibTIFF 3.x](http://www.libtiff.org)
* [FFTW 3.x](http://www.fftw.org/download.html)
* [PHYLIP](http://evolution.genetics.washington.edu/phylip/install.html)

Test Images:
-----
A set of test images from the [IICBU Biological Image Repository](http://ome.grc.nia.nih.gov/iicbu2008) is automatically
loaded into to the virtual machine when it is launched.

To Run wnd-chrm:
-----
With the vagrant running connect to it with ssh:
<pre>$ vagrant ssh  # should work on Mac OS X, Linux, and some Windows configurations</pre>
  
Use an SSH utility if SSH is not supported from the command line on your system.
  
- Host: 127.0.0.1
- Port: 2222
- Username: vagrant
- Password: vagrant
    
From the SSH prompt the wnd-chrm commands can be entered.

<pre>$ wndchrm train \[options\] *images* *feature_file*
$ wndcharm test \[options\] *feature_file* \[report_file\]
$ wndchrm classify *feature_file* *image*</pre>

Use an SSH utility if SSH is not supported from the command line on your system.
  
- Host: 127.0.0.1
- Port: 2222
- Username: vagrant
- Password: vagrant
    
From the SSH prompt the wnd-chrm commands can be entered.

<pre>$ wndchrm train \[options\] *images* *feature_file*
$ wndcharm test \[options\] *feature_file* \[report_file\]
$ wndchrm classify *feature_file* *image*</pre>

    
A full description of wndchrm including usage of the above commands:
  
[Shamir L, Orlov N, Eckley DM, Macura T, Johnston J, Goldberg IG. Wndchrm - an open source utility for biological image analysis.](http://www.scfbm.org/content/3/1/13) BMC Source Code for Biology and Medicine. 3: 13, 2008. [PDF download](http://ome.grc.nia.nih.gov/wnd-charm/BMC-wndchrm-utility.pdf)
    
    
  


