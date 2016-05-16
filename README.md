# Instructions for VATIC installation

[VATIC](http://web.mit.edu/vondrick/vatic/) is a free, online, interactive video annotation tool for computer vision research that crowdsources work to Amazon’s Mechanical Turk. It can be used in offline mode for expert annotator use as well, and is an optimized tool for video annotation.

There is already a default README on their website, but I was unable to install it only following the default instructions, so here I wrote what issues I encountered during installation what I did to install it successfully.

#### Basic configuration of my machine
* Ubuntu 14.04


#### Issues I encountered
1. Packages Missing Problem
 * Before running the downloaded .sh file, you need to take the following steps:<br>
        _sudo apt-get update <br>
        sudo apt-get install python-setuptools<br>
        sudo apt-get install git<br>
        sudo apt-get install build-essential<br>
        sudo apt-get install autoconf libtool pkg-config python-opengl python-imaging pythonpyrex
        python-pyside.qtopengl idle-python2.7 qt4-dev-tools qt4-designer libqtgui4
        libqtcore4 libqt4-xml libqt4-test libqt4-script libqt4-network libqt4-dbus python-qt4
        python-qt4-gl libgle3 python-dev
        sudo apt-get install libapache2-mod-wsgi<br>
        sudo a2enmod mod-wsgi<br>
        sudo apt-get install python-mysqldb<br>
        sudo easy install munkres<br>
        sudo apt-get install python-pip<br>
        sudo pip install parsedatetime<br>_

 * Then in order to be able to process jpeg files, you also need to install libjpeg-dev with apt:<br>
        _sudo apt-get install libjpeg-dev<br>
        pip install -I pillow<br>_

 * Then reinstall pillow:<br>
        _pip install -I pillow_

 * Then you can follow the original instructions to continue.

2. Mysql

3. vatic location

4. sudo apache2ctl restart
   
