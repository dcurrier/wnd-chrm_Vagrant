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

Test Images
-----
A set of test images from the [IICBU Biological Image Repository](http://ome.grc.nia.nih.gov/iicbu2008) are included in the repository.  


