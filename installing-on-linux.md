# Installing Anaconda on Linux

## Download Anaconda

### From Anaconda site
1. Download Anaconda installer for Linux from here: [https://www.anaconda.com/download/](https://www.anaconda.com/download/)
2. Choose ``Python 2.7`` or ``Python 3.6``, read
[python2 vs python3](./python2-vs-python3.md)

### From Anaconda repository
1. Download Anaconda installer for Linux from here: https://repo.continuum.io/archive/ using ``wget``
or from the browser.
2. If you choose to use wget, check the latest version ``X.X.X``, open up a terminal and replace the X.X.X with the latest version.
3. For Python 2.7 :
``wget http://repo.continuum.io/archive/Anaconda2-X.X.X-Linux-x86_64.sh``
4. for Python 3.x:
``wget http://repo.continuum.io/archive/Anaconda3-5.0.1-Linux-x86_64.sh``

## Installing Anaconda
1. Open up a terminal.
2. ``cd`` to your instaler folder.
3. Type ``sh ./AnacondaXXXXXXXX.sh``, where ``AnacondaXXXXXXXX.sh`` refers to the downloaded file name.
4. Follow the instructions on the screen. Accept the
defaults if you are not sure what to do :stuck_out_tongue:.
5. Installation will be finished within 5 minutes.
6. The following line will be appeared:
``Do you wish the installer to prepend the AnacondaX install location to PATH in your /home/XXX/.bashrc ? [yes|no]``
7. If you use ``bash``, you can type ``yes`` for easy installation. Read the next session about ``PATH variable``
8. Everything is done. Refresh your bash terminal by ``source ~/.bashrc`` 

## Anaconda ``PATH`` variable
The Anaconda will **NOT** append the ``PATH`` variable during Linux installation. To qurantee your installation is successful, you need to check your rcfile for Bash, i.e. the ``.bashrc`` stored under the Home directory of Linux. To read the ``.bashrc``:
1. Type ``cat ~/.bashrc`` in your terminal.
2. If you have the following lines at the end, it means the installation is ok.
```
# added by Anaconda2 installer
export PATH="/home/XXXXX/anacondaX/bin:$PATH"
```
3. If you doesn't got this line, first check the Anaconda installation location (usually /home/XXXXX/anacondaX/) and add the following line (Replace /home/XXXXX/anacondaX/ with your installation location) to ``~/.bashrc`` using a text editor:
```
export PATH="/home/XXXXX/anacondaX/bin:$PATH"
```
4. If you have no idea what is a text editor, open a terminal,
type ``echo "export PATH="/home/XXXXX/anacondaX/bin:$PATH"" >> ~/.bashrc`` and enter, ofcourse replace your installation folder here.

## Successful Anaconda installation
1. Run ``source ~/.bashrc`` in the terminal.
2. Type ``python`` in the terminal.
3. Similar strings will be appeared: :heavy_check_mark:
```
Python 2.7.14 |Anaconda custom (64-bit)| (default, Oct 16 2017, 17:29:19) 
[GCC 7.2.0] on linux2
Type "help", "copyright", "credits" or "license" for more information. 
```
4. If the following similar strings appeared, redo the previous session or run ``source ~/.bashrc`` in the terminal. :heavy_multiplication_x:
```
Python 2.7.14 (default, Jan  5 2018, 10:41:29) 
[GCC 7.2.1 20171224] on linux2
Type "help", "copyright", "credits" or "license" for more information.
```

## Updating conda

1. Open a terminal.
2. Run ``conda update anaconda``.

## Uninstalling conda

1. Open a terminal.
2. Check the Anaconda installation path.
3. Usually ``~/anacondaX/``
4. Run ``rm -fr ~/anacondaX/``
5. Open your ``~/.bashrc``
6. Find and remove the line ``export PATH="/home/XXXXX/anacondaX/bin:$PATH"``
7. Run ``source ~/.bashrc``